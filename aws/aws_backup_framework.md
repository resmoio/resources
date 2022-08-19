---
description: Amazon Web Services Backup Framework
---
aws_backup_framework
--------------------

| **Name**         | **Type**               | **Nullable** |
| ---------------- | ---------------------- | ------------ |
| accountId        | String                 | &cross;      |
| accountName      | String                 | &check;      |
| arn              | String                 | &cross;      |
| controls         | List<FrameworkControl> | &check;      |
| creationTime     | String                 | &check;      |
| deploymentStatus | String                 | &cross;      |
| description      | String                 | &check;      |
| idempotencyToken | String                 | &check;      |
| name             | String                 | &cross;      |
| region           | String                 | &cross;      |
| status           | String                 | &cross;      |

#### FrameworkControl
| **Name**        | **Type**                                     | **Nullable** |
| --------------- | -------------------------------------------- | ------------ |
| inputParameters | List<FrameworkControl.ControlInputParameter> | &check;      |
| name            | String                                       | &cross;      |
| scope           | FrameworkControl.ControlScope                | &check;      |

#### FrameworkControl.ControlInputParameter
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| value    | String   | &cross;      |

#### FrameworkControl.ControlScope
| **Name**                | **Type**           | **Nullable** |
| ----------------------- | ------------------ | ------------ |
| complianceResourceIds   | List<String>       | &check;      |
| complianceResourceTypes | List<String>       | &check;      |
| tags                    | Map<String,String> | &check;      |
