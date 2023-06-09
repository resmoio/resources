---
description: GitHub Actions Repository Secret
---
github_actions_repo_secret
--------------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| createdAt    | String       | &cross;      |
| name         | String       | &cross;      |
| organization | Organization | &cross;      |
| repository   | Repository   | &cross;      |
| updatedAt    | String       | &cross;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
