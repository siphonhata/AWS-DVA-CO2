# Synchronous vs Asynchronous

When designing communication between services, you need to decide whether it should be synchronous or asynchronous.

## Synchronous
In synchronous communication, the caller waits for a response before proceeding.

Example: Making an **API Gateway** request and waiting for the result is a synchronous operation.

## Asynchronous
Asynchronous communication allows the caller to continue processing without waiting for the response.

Example: **SNS** and **SQS** allow for asynchronous messaging, where services process messages independently.

