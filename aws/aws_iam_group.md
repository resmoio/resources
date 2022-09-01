---
description: Amazon Web Services IAM Group
---
aws_iam_group
-------------

| **Name**         | **Type**             | **Nullable** |
| ---------------- | -------------------- | ------------ |
| accountId        | String               | &cross;      |
| accountName      | String               | &check;      |
| arn              | String               | &check;      |
| attachedPolicies | List<AttachedPolicy> | &cross;      |
| id               | String               | &cross;      |
| name             | String               | &cross;      |
| path             | String               | &check;      |
| policies         | List<GroupPolicy>    | &cross;      |

#### AttachedPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &cross;      |
| name     | String   | &cross;      |

#### GroupPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| document | JSON     | &check;      |
| name     | String   | &cross;      |
