---
description: Amazon Web Services SSM Parameter
---
aws_ssm_parameter
-----------------

| **Name**         | **Type**                    | **Nullable** |
| ---------------- | --------------------------- | ------------ |
| accountId        | String                      | &cross;      |
| accountName      | String                      | &check;      |
| allowedPattern   | String                      | &check;      |
| dataType         | String                      | &check;      |
| description      | String                      | &check;      |
| keyId            | String                      | &check;      |
| lastModifiedDate | String                      | &check;      |
| lastModifiedUser | String                      | &check;      |
| name             | String                      | &cross;      |
| policies         | List<ParameterInlinePolicy> | &check;      |
| region           | String                      | &cross;      |
| tier             | String                      | &check;      |
| type             | String                      | &check;      |
| version          | Long                        | &check;      |

#### ParameterInlinePolicy
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| policyStatus | String   | &check;      |
| policyText   | String   | &check;      |
| policyType   | String   | &check;      |
