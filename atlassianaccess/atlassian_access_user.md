---
description: Atlassian Access User
---
atlassian_access_user
---------------------

| **Name**       | **Type**            | **Nullable** |
| -------------- | ------------------- | ------------ |
| accessBillable | Boolean             | &check;      |
| accountId      | String              | &cross;      |
| accountStatus  | String              | &check;      |
| accountType    | String              | &check;      |
| email          | String              | &check;      |
| lastActive     | String              | &check;      |
| name           | String              | &check;      |
| organizationId | String              | &cross;      |
| picture        | String              | &check;      |
| productAccess  | List<ProductAccess> | &check;      |

#### ProductAccess
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| key        | String   | &check;      |
| lastActive | String   | &check;      |
| name       | String   | &check;      |
| url        | String   | &check;      |
