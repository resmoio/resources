---
description: Amazon Web Services IAM Role
---
aws_iam_role
------------

| **Name**         | **Type**             | **Nullable** |
| ---------------- | -------------------- | ------------ |
| accountId        | String               | &cross;      |
| accountName      | String               | &check;      |
| arn              | String               | &cross;      |
| assumeRolePolicy | JSON                 | &check;      |
| attachedPolicies | List<AttachedPolicy> | &cross;      |
| id               | String               | &cross;      |
| name             | String               | &cross;      |
| policies         | List<Policy>         | &cross;      |
| tags             | Map<String,String>   | &cross;      |

#### AttachedPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &cross;      |
| name     | String   | &cross;      |

#### Policy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| document | JSON     | &check;      |
| name     | String   | &cross;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

