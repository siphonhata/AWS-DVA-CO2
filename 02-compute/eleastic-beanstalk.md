# 📘 AWS Elastic Beanstalk (EB) Summary – DVA-C02

---

## 🔍 What is Elastic Beanstalk?

**Elastic Beanstalk** is a **Platform-as-a-Service (PaaS)** that enables you to deploy and scale web applications and services without managing the underlying infrastructure.

- Automatically handles: **EC2**, **Load Balancer**, **Auto Scaling**, **RDS**, **CloudWatch**
- Supports multiple programming languages and Docker

---

## 🧱 Core Features

| Feature                    | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| **PaaS**                   | Simplifies deployment without managing infra                                |
| **Multi-Language Support**| Java, .NET, Node.js, Python, PHP, Ruby, Go, Docker                          |
| **Managed Environment**   | Provisions EC2, ELB, RDS, Auto Scaling, etc.                                |
| **Configurable**          | Use EB CLI or `.ebextensions/` for setup                                    |
| **Monitoring**            | Integrated with CloudWatch and health dashboard                            |
| **Version Control**       | Supports rollbacks and app version tracking                                 |

---

## 🧰 Components Involved

| Component      | Purpose                                                       |
|----------------|---------------------------------------------------------------|
| **EC2**         | Runs the application                                          |
| **S3**          | Stores application versions and logs                         |
| **CloudWatch**  | Monitors logs and metrics                                    |
| **ELB**         | Load balances across EC2 instances                           |
| **Auto Scaling**| Automatically scales up/down instances                       |
| **RDS (Optional)**| Deploys a database along with your app (use with caution) |

---

## 🚀 Deployment Strategies

| Strategy                      | Description                                                              |
|-------------------------------|--------------------------------------------------------------------------|
| **All at Once**               | Fast, deploys to all instances—risk of downtime                          |
| **Rolling**                   | Deploys in batches, maintains availability                               |
| **Rolling w/ Additional Batch**| Adds temp capacity during deploy                                         |
| **Immutable**                 | Spins up new instances and swaps if healthy                              |
| **Blue/Green**                | Deploy to a new env, switch DNS—zero downtime                            |

---

## ⚙️ Configuration Options

| Item                        | Description                                                |
|-----------------------------|------------------------------------------------------------|
| **Environment Variables**   | Set secrets or runtime configuration                      |
| **`.ebextensions/`**        | Folder with `.config` files for advanced setup            |
| **Environment Types**       | Web Server or Worker environments                         |
| **Platform Versions**       | Use AWS-maintained runtime platforms                      |

---

## 🧪 Common EB CLI Commands

| Command          | Description                                   |
|------------------|-----------------------------------------------|
| `eb init`        | Initialize a new EB app                       |
| `eb create`      | Create a new environment                      |
| `eb deploy`      | Deploy current app version                    |
| `eb open`        | Opens your app in the browser                 |
| `eb logs`        | Fetch logs from the environment               |
| `eb config`      | View or edit configuration                    |
| `eb terminate`   | Delete the environment                        |

---

## ✅ Best Practices

| Practice                             | Reason                                               |
|--------------------------------------|------------------------------------------------------|
| Use **Immutable** or **Blue/Green**  | Safer, zero-downtime deployments                     |
| Store secrets in **SSM or Secrets Manager** | Secure key handling                         |
| Use `.ebextensions/`                 | Automate app setup                                  |
| Separate **RDS** from EB lifecycle   | Prevent accidental DB deletion                      |
| Monitor with **CloudWatch**          | Track health, performance, and auto-scaling         |

---

## 📘 Example Use Cases (Exam-Ready)

- Deploy a **Python Flask** or **Node.js Express** app quickly
- Handle **Auto Scaling** based on traffic spikes
- Monitor application **health and logs** in CloudWatch
- Integrate with **CI/CD** using CodePipeline or GitHub Actions
- Implement **Blue/Green deployments** to avoid downtime

---

