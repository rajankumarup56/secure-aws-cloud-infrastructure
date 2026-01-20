# OTP Email System

## Purpose
To send secure OTP emails to users for authentication.

## Architecture Flow
1. **User** triggers OTP request.
2. **SNS** receives event from application (decoupling & buffering).
3. **SQS** queues the OTP event (retry & fault tolerance).
4. **Lambda** processes the message and generates OTP.
5. **SES** sends the OTP email to the user.

## AWS Services Used
- Amazon SNS
- Amazon SQS
- AWS Lambda
- Amazon SES
- IAM (for permissions)
- CloudWatch (monitoring)

## Outcome
- Reliable OTP delivery
- Scalable and fault-tolerant
- Event-driven architecture demonstrated
