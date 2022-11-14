---
description: Amazon Web Services CloudFormation Stack
---
aws_cloudformation_stack
------------------------

| **Name**                    | **Type**              | **Nullable** |
| --------------------------- | --------------------- | ------------ |
| accountId                   | String                | &cross;      |
| accountName                 | String                | &check;      |
| capabilities                | List<String>          | &check;      |
| changeSetId                 | String                | &check;      |
| creationTime                | String                | &check;      |
| deletionTime                | String                | &check;      |
| description                 | String                | &check;      |
| disableRollback             | Boolean               | &check;      |
| enableTerminationProtection | Boolean               | &check;      |
| id                          | String                | &cross;      |
| name                        | String                | &check;      |
| notificationArns            | List<String>          | &check;      |
| outputs                     | List<String>          | &check;      |
| parentId                    | String                | &check;      |
| region                      | String                | &cross;      |
| roleArn                     | String                | &check;      |
| rollbackConfiguration       | RollbackConfiguration | &check;      |
| rootId                      | String                | &check;      |
| status                      | String                | &check;      |
| statusReason                | String                | &check;      |
| timeoutInMinutes            | Int                   | &check;      |

#### Output
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| exportName  | String   | &check;      |
| key         | String   | &cross;      |
| value       | String   | &cross;      |

#### RollbackConfiguration
| **Name**                | **Type**                                    | **Nullable** |
| ----------------------- | ------------------------------------------- | ------------ |
| hasRollbackTriggers     | Boolean                                     | &cross;      |
| monitoringTimeInMinutes | Int                                         | &check;      |
| rollbackTriggers        | List<RollbackConfiguration.RollbackTrigger> | &cross;      |

#### RollbackConfiguration.RollbackTrigger
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &cross;      |
| type     | String   | &cross;      |
