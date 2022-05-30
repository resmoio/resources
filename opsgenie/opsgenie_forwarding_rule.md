---
description: Opsgenie Forwarding Rule
---
opsgenie_forwarding_rule
------------------------

| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| accountName | String   | &check;      |
| alias       | String   | &cross;      |
| endDate     | Date     | &check;      |
| fromUser    | User     | &check;      |
| id          | String   | &cross;      |
| startDate   | Date     | &check;      |
| toUser      | User     | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| username | String   | &check;      |
