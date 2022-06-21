---
description: GitHub Organization Member
---
github_org_member
-----------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| organization | Organization | &check;      |
| role         | String       | &cross;      |
| state        | String       | &cross;      |
| user         | User         | &cross;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
