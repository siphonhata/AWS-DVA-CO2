# 📘 AWS Certified Developer – Associate (DVA-C02) Learning Journey

Welcome to my learning repository for the AWS DVA-C02 certification! 🎓

This repo documents everything I’m studying, practicing, and building along the way — from theory to labs, diagrams, and hands-on experiments.

---

## 📚 Topics Covered

- [x] IAM & Security
- [x] Compute: EC2, Lambda, Elastic Beanstalk
- [x] Storage: S3, EFS, Glacier
- [x] Databases: RDS, DynamoDB
- [x] Networking: VPC, API Gateway, App Load Balancer
- [x] Dev Tools: CodeCommit, CodeBuild, CodeDeploy, CodePipeline
- [x] Monitoring & Logging: CloudWatch, X-Ray
- [x] CI/CD Best Practices
- [x] Exam Tips & Practice Questions

---

## 🗂️ Repo Structure

```bash
aws-dva-c02-learning-journey/
domain-1-development-with-aws-services/
├── README.md                              # Overview of domain 1 with a summary of the services covered
├── develop-code-for-applications-hosted-on-aws/
│   ├── README.md                          # Introduction to developing applications hosted on AWS
│   ├── architectural-patterns.md          # Architectural patterns for AWS-hosted applications
│   ├── idempotency.md                     # Idempotency in distributed applications
│   ├── stateful-vs-stateless.md           # Difference between stateful and stateless architectures
│   ├── fault-tolerant-design.md           # Best practices for designing fault-tolerant applications
│   ├── synchronous-asynchronous.md        # When to use synchronous vs asynchronous operations
│   ├── coding-for-resilience.md           # Writing resilient code to handle failures
│   ├── apis.md                            # Building APIs using AWS services (API Gateway, Lambda, etc.)
│   ├── unit-testing.md                    # Unit testing strategies for Lambda, APIs, and other AWS services
│   ├── messaging.md                       # Working with messaging services (SQS, SNS)
│   ├── sdk.md                             # Using the AWS SDK for different programming languages (Python, Node.js, 
│   └── streaming.md                       # Using AWS services for streaming data (e.g., Kinesis)
├── develop-code-for-aws-lambda/
│   ├── README.md                          # Introduction to developing AWS Lambda functions
│   ├── lambda-basics.md                   # Basics of Lambda functions, triggers, and events
│   ├── lambda-deployment.md               # How to deploy and manage Lambda functions
│   ├── lambda-performance.md              # Performance tuning for Lambda functions
│   ├── lambda-versions-and-aliases.md     # Using versions and aliases for Lambda
│   ├── lambda-best-practices.md           # Best practices for writing efficient Lambda functions
│   └── lambda-debugging.md                # Debugging techniques for Lambda functions
├── use-data-stores-in-application-development/
│   ├── README.md                          # Introduction to using data stores with AWS applications
│   ├── dynamodb.md                        # Working with DynamoDB (CRUD operations, indexing, design patterns)
│   ├── s3.md                              # Using S3 for object storage (uploads, permissions, lifecycle)
│   ├── rds.md                             # Using RDS for relational databases (PostgreSQL, MySQL, etc.)
│   ├── redshift.md                        # Using Redshift for data warehousing and analytics
│   ├── aurora.md                          # Working with Amazon Aurora for scalable database solutions
│   └── elasticache.md                     # Using ElastiCache for in-memory data stores (Redis, Memcached)
├── security-best-practices.md             # Security practices in AWS (IAM roles, encryption, access control)
├── scalability-and-cost-management.md     # Scaling and cost management in AWS (autoscaling, cost optimization)
├── ci-cd-pipelines.md                    # Setting up CI/CD pipelines for Lambda and AWS services
├── sns-sqs-integration.md                # Integrating messaging services (SNS, SQS)
├── serverless-framework.md               # Using Serverless Framework to deploy applications on AWS
├── monitoring-logging.md                 # Monitoring Lambda functions and AWS  using CloudWatch and CloudTrail
├──domain-2-security-and-data-protection/
├── README.md                                  # Overview of Domain 2, covering security and data protection in AWS
├── implement-authentication-and-authorization/
│   ├── README.md                              # Introduction to implementing authentication and authorization in AWS
│   ├── iam-basics.md                          # Introduction to AWS Identity and Access Management (IAM)
│   ├── creating-iam-roles.md                  # Creating IAM roles, users, and policies
│   ├── aws-cognito.md                        # Using AWS Cognito for user authentication and authorization
│   ├── federated-identity.md                  # Implementing federated identities using AWS services (Cognito, SSO)
│   ├── oauth-2-0.md                          # Implementing OAuth 2.0 for securing APIs
│   ├── aws-sso.md                            # Configuring AWS Single Sign-On (SSO) for centralized access
│   ├── access-control-policies.md            # Writing IAM policies for fine-grained access control
│   ├── multi-factor-authentication.md         # Enabling MFA for added security
│   ├── api-gateway-authorization.md          # Securing APIs using API Gateway and Lambda Authorizers
│   └── service-to-service-authentication.md  # Service-to-service authentication with IAM roles and policies
├── implement-encryption-using-aws-services/
│   ├── README.md                              # Introduction to encryption using AWS services
│   ├── kms.md                                 # Using AWS Key Management Service (KMS) for encryption and key
│   ├── ssm-parameter-store.md                 # Using AWS SSM Parameter Store to manage secrets and configurations
│   ├── secrets-manager.md                     # Using AWS Secrets Manager for storing and managing sensitive 
│   ├── encrypting-data-in-transit.md          # Encrypting data in transit with TLS/SSL (e.g., API Gateway, S3)
│   ├── encrypting-data-at-rest.md             # Encrypting data at rest with S3, EBS, RDS, etc.
│   ├── cloudhsm.md                            # Using AWS CloudHSM for hardware-based encryption solutions
│   └── encryption-best-practices.md           # Best practices for implementing encryption in AWS
├── manage-sensitive-data-in-application-code/
│   ├── README.md                              # Introduction to managing sensitive data securely in application code
│   ├── secure-coding-practices.md             # Secure coding practices for handling sensitive data
│   ├── environment-variables.md               # Using environment variables to store sensitive data
│   ├── encryption-in-code.md                  # Encrypting sensitive data within application code
│   ├── secure-credentials-management.md       # Managing credentials in application code using IAM roles, SSM, 
│   ├── avoiding-hardcoded-secrets.md          # Best practices for avoiding hardcoded secrets in code
│   ├── logging-sensitive-data.md              # Handling sensitive data in logs and ensuring compliance
│   └── audit-and-monitoring.md                # Auditing and monitoring access to sensitive data and encryption keys

├── domain-3-application-deployment-testing-and-automation-on-aws/
├── README.md                              # Overview of Domain 3 with a summary of services covered
├── prepare-application-artifacts-for-aws-deployment/
│   ├── README.md                          # Introduction to preparing application artifacts for AWS deployment
│   ├── artifact-packaging.md              # How to package application code, dependencies, and configuration
│   ├── lambda-deployment.md               # Deploying Lambda functions with packaged artifacts
│   ├── docker-containers.md               # Containerizing applications for AWS (ECS, EKS, Lambda)
│   ├── s3-artifacts.md                    # Storing and managing application artifacts in S3 for deployment
│   └── codebuild-artifacts.md             # Using CodeBuild to prepare artifacts for deployment
├── test-applications-in-development-environments/
│   ├── README.md                          # Introduction to testing applications in development environments
│   ├── local-testing.md                   # Techniques for testing applications locally (SAM CLI, LocalStack)
│   ├── integration-testing.md             # Setting up integration tests with AWS services (API Gateway, Lambda)
│   ├── unit-testing.md                    # Unit testing strategies for Lambda, APIs, and other AWS services
│   ├── mocking-aws-services.md            # Mocking AWS services for local development (LocalStack, Moto)
│   ├── debugging.md                       # Debugging applications in local or test environments
│   └── cloud9-environment.md             # Using AWS Cloud9 for cloud-based development and testing
├── automate-deployment-testing/
│   ├── README.md                          # Introduction to automating deployment testing
│   ├── ci-cd-testing.md                   # Automating tests in CI/CD pipelines (CodePipeline, CodeBuild)
│   ├── test-automation-tools.md           # Tools and frameworks for automating tests (JUnit, Mocha, etc.)
│   ├── infrastructure-testing.md          # Testing AWS infrastructure using tools like CloudFormation, Terraform
│   ├── end-to-end-testing.md              # Setting up end-to-end tests for AWS deployments (AWS Device Farm, Selenium)
│   ├── test-reporting.md                  # Analyzing test results and reporting (CloudWatch, AWS X-Ray)
│   └── continuous-testing.md              # Implementing continuous testing in CI/CD workflows
├── deploy-code-using-aws-ci-cd-services/
│   ├── README.md                          # Introduction to deploying code using AWS CI/CD services
│   ├── codepipeline-overview.md           # Overview of AWS CodePipeline for continuous integration and deployment
│   ├── codebuild-deployment.md            # Using AWS CodeBuild for building and deploying applications
│   ├── codedeploy-deployment.md           # Deploying applications with AWS CodeDeploy
│   ├── cloudformation-deployment.md      # Deploying applications using AWS CloudFormation
│   ├── automated-deployment.md           # Setting up fully automated deployments (push to production)
│   ├── pipeline-best-practices.md         # Best practices for setting up and managing CI/CD pipelines
│   └── rollbacks-and-failures.md          # Handling rollbacks and failures in the CI/CD process

├── domain-4-root-cause-analysis-and-observability-on-aws/
├── README.md                              # Overview of Domain 4 with a summary of services covered
├── assist-in-root-cause-analysis/
│   ├── README.md                          # Introduction to root cause analysis (RCA) in AWS environments
│   ├── RCA-methodologies.md               # Common methodologies for performing root cause analysis (5 Whys, Fishbone)
│   ├── logs-for-rca.md                    # Using AWS CloudWatch logs to identify issues
│   ├── cloudtrail-for-rca.md              # Analyzing AWS CloudTrail logs to understand API activity
│   ├── monitoring-and-alerting.md         # Setting up CloudWatch alarms to detect failures
│   ├── troubleshooting-techniques.md      # General troubleshooting techniques for AWS services (EC2, Lambda, etc.)
│   └── case-study.md                      # A case study on performing RCA for a failure in an AWS environment
├── instrument-code-for-observability/
│   ├── README.md                          # Introduction to instrumenting code for observability in AWS environments
│   ├── cloudwatch-metrics.md              # Creating and using CloudWatch metrics for application performance
│   ├── cloudwatch-logs.md                 # Implementing CloudWatch Logs for capturing application logs
│   ├── cloudwatch-logs-insights.md        # Analyzing logs using CloudWatch Logs Insights
│   ├── x-ray-tracing.md                  # Setting up AWS X-Ray for tracing and debugging applications
│   ├── custom-metrics.md                  # Creating custom CloudWatch metrics for more granular monitoring
│   ├── monitoring-best-practices.md       # Best practices for setting up observability in cloud-based applications
│   └── error-handling-and-alerting.md     # Setting up error handling and alerting to quickly detect and address issues
├── implement-authentication-authorization-for-applications-and-aws-services/
│   ├── README.md                          # Introduction to implementing authentication and authorization on AWS
│   ├── iam-roles.md                       # Using AWS IAM roles to manage authentication and authorization
│   ├── cognito.md                         # Implementing Amazon Cognito for user authentication
│   ├── federated-identity.md              # Implementing federated authentication (SSO, social login) with Cognito
│   ├── api-gateway-authorization.md       # Using API Gateway for API authentication and authorization (IAM, Lambda authorizers)
│   ├── encryption-and-access-control.md   # Implementing encryption and access control (KMS, S3 bucket policies)
│   ├── aws-iam-best-practices.md          # Best practices for managing IAM roles, policies, and permissions
│   └── oauth-openid-connect.md            # Using OAuth and OpenID Connect for secure authentication in web apps

├── practice-questions/
│   ├── domain-1.md
│   ├── domain-2.md
│   ├── domain-3.md
│   └── domain-4.md
├── notes/
│   └── cheatsheets/
│       ├── s3-vs-efs-vs-efs-infrequent.md
│       ├── lambda-vs-ec2-vs-eb.md
│       └── cloudwatch-vs-cloudtrail.md
└── resources/
    ├── study-plan.md
    └── useful-links.md


