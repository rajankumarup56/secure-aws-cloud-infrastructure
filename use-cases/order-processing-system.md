# Order Processing System

## Purpose
To send order confirmation emails when a user places an order.

## Architecture Flow
1. **User** places an order.
2. **SNS** publishes order event.
3. **SQS** queues the event for processing.
4. **Lambda** reads event, formats email, triggers SES.
5. **SES** sends confirmation email to the user.

## Outcome
- Reliable email confirmations
- Handles traffic spikes safely
- Demonstrates event-driven architecture
