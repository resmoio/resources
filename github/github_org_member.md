---
description: GitHub Organization Member
---
github_org_member
-----------------

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| organizationId | String   | &cross;      |
| role           | String   | &cross;      |
| state          | String   | &cross;      |
| user           | User     | &cross;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &cross;      |
| login    | String   | &cross;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
