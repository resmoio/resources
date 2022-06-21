---
description: GitHub Team Member
---
github_team_member
------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| organization | Organization | &check;      |
| role         | String       | &cross;      |
| state        | String       | &cross;      |
| team         | Team         | &check;      |
| user         | User         | &cross;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &cross;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
