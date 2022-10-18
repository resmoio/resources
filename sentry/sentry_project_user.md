---
description: Sentry Project User
---
sentry_project_user
-------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| dateCreated  | String       | &check;      |
| email        | String       | &check;      |
| hash         | String       | &check;      |
| id           | String       | &cross;      |
| identifier   | String       | &check;      |
| ipAddress    | String       | &check;      |
| name         | String       | &check;      |
| organization | Organization | &check;      |
| project      | Project      | &check;      |
| tagValue     | String       | &check;      |
| username     | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &check;      |
