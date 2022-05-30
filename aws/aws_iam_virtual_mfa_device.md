---
description: Amazon Web Services IAM Virtual MFA Device
---
aws_iam_virtual_mfa_device
--------------------------

| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| accountId    | String   | &cross;      |
| enableDate   | String   | &check;      |
| serialNumber | String   | &cross;      |
| user         | User     | &check;      |

#### User
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| arn        | String   | &check;      |
| createDate | String   | &check;      |
| userId     | String   | &check;      |
| userName   | String   | &check;      |
