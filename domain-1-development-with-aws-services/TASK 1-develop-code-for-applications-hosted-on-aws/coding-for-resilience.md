# Coding for Resilience

Resilient applications can tolerate and recover from failures without impacting user experience. AWS provides several tools and services to help build resilient applications.

## Fault Tolerance with AWS
- **AWS Lambda** allows automatic retries with exponential backoff for transient failures.
- **Amazon S3** ensures data durability and availability by replicating data across multiple facilities.
- **Amazon RDS** offers multi-AZ deployments to improve availability and resilience.

## Resilient Code Practices
- Implement retry logic with **exponential backoff** for better handling of network issues.
- Use **Dead Letter Queues (DLQs)** for failed messages in **SQS** to ensure no data loss.
- Use **circuit breakers** to prevent overwhelming services in case of failure.

