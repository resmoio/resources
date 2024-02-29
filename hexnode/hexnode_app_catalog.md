---
description: Hexnode App Catalog
---
hexnode_app_catalog
-------------------

| **Name**     | **Type**       | **Nullable** |
| ------------ | -------------- | ------------ |
| app_groups   | List<AppGroup> | &check;      |
| apps         | List<App>      | &check;      |
| created_time | String         | &check;      |
| description  | String         | &check;      |
| id           | Int            | &cross;      |
| name         | String         | &check;      |

#### App
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| category  | String   | &check;      |
| id        | Int      | &cross;      |
| name      | String   | &check;      |
| price     | String   | &check;      |
| publisher | String   | &check;      |

#### AppGroup
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | Int      | &cross;      |
| name        | String   | &check;      |
