# Fault-Tolerant Design Patterns

Building fault-tolerant systems ensures that applications can continue to function even in the event of partial failures. This is especially important in cloud architectures where services may occasionally experience issues.

## Retries with Exponential Backoff and Jitter
Exponential backoff and jitter help prevent retries from overwhelming a system during a failure. AWS SDKs use this pattern by default for retries, and you can implement it in your applications to handle retries more effectively.

## Dead Letter Queues (DLQ)
When a message cannot be processed after a certain number of attempts, it is sent to a **Dead Letter Queue** for later inspection. This ensures that messages are not lost but can be processed later.

## Graceful Degradation
When a failure occurs, design your system to degrade gracefully, providing limited functionality rather than complete failure.

