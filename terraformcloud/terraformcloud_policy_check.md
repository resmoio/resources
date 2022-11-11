---
description: Terraform Cloud Policy Check
---
terraformcloud_policy_check
---------------------------

| **Name**    | **Type**            | **Nullable** |
| ----------- | ------------------- | ------------ |
| id          | String              | &cross;      |
| permissions | Map<String,Boolean> | &check;      |
| result      | Result              | &check;      |
| scope       | String              | &check;      |
| status      | String              | &check;      |
| type        | String              | &check;      |
| workspaceId | String              | &check;      |

#### Result
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| advisoryFailed | Int      | &check;      |
| hardFailed     | Int      | &check;      |
| passed         | Int      | &check;      |
| result         | Boolean  | &check;      |
| softFailed     | Int      | &check;      |
| totalFailed    | Int      | &check;      |
