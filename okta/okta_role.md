---
description: Okta Role
---
okta_role
---------

| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| created     | String           | &check;      |
| description | String           | &check;      |
| id          | String           | &cross;      |
| label       | String           | &check;      |
| lastUpdated | String           | &check;      |
| permissions | List<Permission> | &check;      |

#### Permission
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| created     | String   | &check;      |
| label       | String   | &check;      |
| lastUpdated | String   | &check;      |
