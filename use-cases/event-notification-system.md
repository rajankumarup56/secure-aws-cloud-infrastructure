# Event Notification System

## Purpose
To send notifications for user actions or system events (alerts, updates).

## Architecture Flow
1. **User / Application** triggers event.
2. **SNS** receives event for broadcasting.
3. **SQS** queues the message for processing.
4. **Lambda** processes message and determines notification content.
5. **SES** sends email notification to intended users.

## Outcome
- Real-time event notifications
- Decoupled and scalable architecture
- Demonstrates understanding of AWS event-driven design
