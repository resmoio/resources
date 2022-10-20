---
description: GitHub Actions Workflow
---
github_actions_workflow
-----------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| createdAt    | String       | &check;      |
| id           | Long         | &cross;      |
| organization | Organization | &cross;      |
| path         | String       | &cross;      |
| repository   | Repository   | &cross;      |
| state        | String       | &check;      |
| updateAt     | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &cross;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
