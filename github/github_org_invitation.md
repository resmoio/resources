---
description: GitHub Organization Invitation
---
github_org_invitation
---------------------

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| createdAt      | Date     | &check;      |
| email          | String   | &check;      |
| failedAt       | Date     | &check;      |
| failedReason   | String   | &check;      |
| id             | Long     | &cross;      |
| inviter        | Inviter  | &check;      |
| login          | String   | &cross;      |
| nodeId         | String   | &check;      |
| organizationId | String   | &cross;      |
| role           | String   | &check;      |
| teamCount      | Int      | &check;      |

#### Inviter
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &cross;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &cross;      |
| login    | String   | &cross;      |
