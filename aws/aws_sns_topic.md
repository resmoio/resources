---
description: Amazon Web Services SNS Topic
---
aws_sns_topic
-------------

| **Name**                              | **Type** | **Nullable** |
| ------------------------------------- | -------- | ------------ |
| accountId                             | String   | &cross;      |
| accountName                           | String   | &check;      |
| application_failure_feedback_role_arn | String   | &check;      |
| arn                                   | String   | &cross;      |
| content_based_deduplication           | Boolean  | &cross;      |
| display_name                          | String   | &check;      |
| effective_delivery_policy             | JSON     | &check;      |
| fifo_topic                            | Boolean  | &cross;      |
| firehose_failure_feedback_role_arn    | String   | &check;      |
| http_failure_feedback_role_arn        | String   | &check;      |
| kmsMasterKeyId                        | String   | &check;      |
| lambda_failure_feedback_role_arn      | String   | &check;      |
| name                                  | String   | &cross;      |
| owner                                 | String   | &check;      |
| policy                                | JSON     | &check;      |
| region                                | String   | &cross;      |
| sqs_failure_feedback_role_arn         | String   | &check;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

