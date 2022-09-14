---
description: Amazon Web Services IAM Identity Center Instance
---
aws_iam_identity_center_instance
--------------------------------

| **Name**                | **Type**                     | **Nullable** |
| ----------------------- | ---------------------------- | ------------ |
| accessControlAttributes | List<AccessControlAttribute> | &check;      |
| accountId               | String                       | &cross;      |
| accountName             | String                       | &check;      |
| arn                     | String                       | &cross;      |
| id                      | String                       | &cross;      |
| region                  | String                       | &cross;      |

#### AccessControlAttribute
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &cross;      |
| value    | List<String> | &check;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

