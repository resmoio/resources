---
description: GitHub Organization Blocked User
---
github_org_blocked_user
-----------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| id           | Long         | &cross;      |
| login        | String       | &check;      |
| nodeId       | String       | &check;      |
| organization | Organization | &check;      |
| siteAdmin    | Boolean      | &check;      |
| type         | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
