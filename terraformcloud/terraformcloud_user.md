---
description: Terraform Cloud User
---
terraformcloud_user
-------------------

| **Name**         | **Type**            | **Nullable** |
| ---------------- | ------------------- | ------------ |
| email            | String              | &check;      |
| id               | String              | &cross;      |
| isServiceAccount | Boolean             | &check;      |
| mfaEnabled       | MfaInfo             | &check;      |
| permissions      | Map<String,Boolean> | &check;      |
| teams            | List<String>        | &check;      |
| type             | String              | &check;      |
| username         | String              | &check;      |
| v2Only           | Boolean             | &check;      |

#### MfaInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |
