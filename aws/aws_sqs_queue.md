---
description: Amazon Web Services SQS Queue
---
aws_sqs_queue
-------------

| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| accountId                    | String   | &cross;      |
| accountName                  | String   | &check;      |
| arn                          | String   | &cross;      |
| createdTimestamp             | String   | &check;      |
| deduplicationScope           | String   | &check;      |
| delaySeconds                 | Int      | &check;      |
| fifoQueue                    | Boolean  | &cross;      |
| fifoThroughputLimit          | String   | &check;      |
| kmsDataKeyReusePeriodSeconds | Int      | &check;      |
| kmsMasterKeyId               | String   | &check;      |
| maxMessageSize               | Int      | &check;      |
| name                         | String   | &cross;      |
| policy                       | JSON     | &check;      |
| region                       | String   | &cross;      |
| retentionPeriod              | Int      | &check;      |
| sqsManagedSseEnabled         | Boolean  | &cross;      |
| visibilityTimeout            | Int      | &check;      |
