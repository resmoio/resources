---
description: GitHub Team Member
---
github_team_member
------------------

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| organizationId | String   | &cross;      |
| role           | String   | &cross;      |
| state          | String   | &cross;      |
| teamId         | Long     | &cross;      |
| user           | User     | &cross;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &cross;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
