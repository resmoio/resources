---
description: SaaS App Account
---
app_account
-----------

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| app            | String   | &check;      |
| approvalReason | String   | &check;      |
| deletedAt      | String   | &check;      |
| domain         | String   | &check;      |
| identifier     | String   | &cross;      |
| isApproved     | Boolean  | &cross;      |
| lastLogin      | String   | &check;      |
| lastUsed       | String   | &check;      |
| loginMethods   | Set      | &check;      |
| owner          | String   | &check;      |

#### LoginType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
| type     | String   | &cross;      |
