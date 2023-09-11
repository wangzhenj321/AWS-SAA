# Amazon Simple Notification Service

Amazon Simple Notification Service (Amazon SNS) is a managed service that provides message delivery from publishers to subscribers (also known as *producers* and *consumers*). Publishers communicate asynchronously with subscribers by sending messages to a *topic*, which is a logical access point and communication channel. Clients can subscribe to the SNS topic and receive published messages using a supported endpoint type, such as Amazon Kinesis Data Firehose, Amazon SQS, AWS Lambda, HTTP, email, mobile push notifications, and mobile text messages (SMS).

![](../imgs/Amazon-Simple-Notification-Service/sns-delivery-protocols.png)

1. [AWS Kinesis vs SNS vs SQS](https://dashbird.io/blog/kinesis-sqs-sns-comparison/)