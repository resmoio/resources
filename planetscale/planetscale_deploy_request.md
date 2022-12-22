---
description: PlanetScale Deploy Request
---
planetscale_deploy_request
--------------------------

| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| actor                   | Actor    | &check;      |
| approved                | Boolean  | &check;      |
| branch                  | String   | &check;      |
| branch_deleted          | Boolean  | &check;      |
| branch_deleted_at       | String   | &check;      |
| branch_deleted_by       | Actor    | &check;      |
| closed_at               | String   | &check;      |
| closed_by               | Actor    | &check;      |
| created_at              | String   | &check;      |
| databaseName            | String   | &check;      |
| deployed_at             | String   | &check;      |
| deployment_state        | String   | &check;      |
| html_body               | String   | &check;      |
| html_url                | String   | &check;      |
| id                      | String   | &cross;      |
| into_branch             | String   | &check;      |
| into_branch_shard_count | Int      | &check;      |
| into_branch_sharded     | Boolean  | &check;      |
| notes                   | String   | &check;      |
| number                  | Int      | &check;      |
| state                   | String   | &check;      |
| updated_at              | String   | &check;      |

#### Actor
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| display_name | String   | &check;      |
| id           | String   | &check;      |
