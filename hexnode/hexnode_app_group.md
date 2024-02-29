---
description: Hexnode App Group
---
hexnode_app_group
-----------------

| **Name**     | **Type**  | **Nullable** |
| ------------ | --------- | ------------ |
| apps         | List<App> | &check;      |
| created_time | String    | &check;      |
| description  | String    | &check;      |
| id           | Int       | &cross;      |
| name         | String    | &check;      |

#### App
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| category  | String   | &check;      |
| id        | Int      | &check;      |
| name      | String   | &check;      |
| price     | String   | &check;      |
| publisher | String   | &check;      |
