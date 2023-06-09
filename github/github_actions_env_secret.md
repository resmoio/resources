---
description: GitHub Actions Environment Secret
---
github_actions_env_secret
-------------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| createdAt    | String       | &cross;      |
| environment  | Environment  | &cross;      |
| name         | String       | &cross;      |
| organization | Organization | &cross;      |
| repository   | Repository   | &cross;      |
| updatedAt    | String       | &cross;      |

#### Environment
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

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
