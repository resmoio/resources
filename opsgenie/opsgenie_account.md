---
description: Opsgenie Account
---
opsgenie_account
----------------

| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| name      | String   | &cross;      |
| plan      | Plan     | &check;      |
| userCount | Int      | &cross;      |

#### Plan
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| isYearly     | Boolean  | &check;      |
| maxUserCount | Int      | &check;      |
| name         | String   | &check;      |
