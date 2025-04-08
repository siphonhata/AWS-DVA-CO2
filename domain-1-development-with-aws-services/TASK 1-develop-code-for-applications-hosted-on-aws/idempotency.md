# Idempotency

Idempotency ensures that repeated executions of an operation yield the same result. This is important for distributed systems to prevent unintended side effects from retries.

## Example in AWS
When an API call is made to create an S3 object, if the same object is uploaded multiple times with the same key, it should not result in multiple objects. You can use **idempotency keys** to achieve this in services like **SQS** and **Lambda**.

## Benefits of Idempotency
- Prevents duplicate processing.
- Ensures consistency and reliability.
- Reduces risk of data corruption.

