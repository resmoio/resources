---
description: Linear User
---
linear_user
-----------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| active            | Boolean      | &check;      |
| admin             | Boolean      | &check;      |
| archivedAt        | String       | &check;      |
| calendarHash      | String       | &check;      |
| createdAt         | String       | &check;      |
| createdIssueCount | Int          | &check;      |
| description       | String       | &check;      |
| disableReason     | String       | &check;      |
| displayName       | String       | &check;      |
| email             | String       | &check;      |
| guest             | Boolean      | &check;      |
| id                | String       | &cross;      |
| inviteHash        | String       | &check;      |
| lastSeen          | String       | &check;      |
| name              | String       | &check;      |
| organization      | Organization | &check;      |
| teams             | Teams        | &check;      |
| timezone          | String       | &check;      |
| updatedAt         | String       | &check;      |
| url               | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |

#### TeamId
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |

#### Teams
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| nodes    | List<TeamId> | &check;      |
