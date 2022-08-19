---
description: Amazon Web Services Organization
---
aws_organization
----------------

| **Name**             | **Type**         | **Nullable** |
| -------------------- | ---------------- | ------------ |
| accountId            | String           | &check;      |
| accountName          | String           | &check;      |
| arn                  | String           | &cross;      |
| availablePolicyTypes | List<PolicyType> | &cross;      |
| featureSet           | String           | &check;      |
| id                   | String           | &cross;      |
| masterAccountArn     | String           | &check;      |
| masterAccountEmail   | String           | &check;      |
| masterAccountId      | String           | &check;      |

#### PolicyType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| status   | String   | &cross;      |
| type     | String   | &cross;      |
