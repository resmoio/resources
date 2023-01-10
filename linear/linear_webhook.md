---
description: Linear Webhook
---
linear_webhook
--------------

| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| allPublicTeams | Boolean      | &check;      |
| archivedAt     | String       | &check;      |
| createdAt      | String       | &check;      |
| creator        | Creator      | &check;      |
| enabled        | Boolean      | &check;      |
| id             | String       | &cross;      |
| label          | String       | &check;      |
| resourceTypes  | List<String> | &check;      |
| secret         | String       | &check;      |
| team           | Team         | &check;      |
| updatedAt      | String       | &check;      |
| url            | String       | &check;      |

#### Creator
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
