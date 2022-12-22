---
description: PlanetScale Database Branch
---
planetscale_database_branch
---------------------------

| **Name**                       | **Type**      | **Nullable** |
| ------------------------------ | ------------- | ------------ |
| access_host_url                | String        | &check;      |
| api_actor                      | Actor         | &check;      |
| created_at                     | String        | &check;      |
| databaseName                   | String        | &check;      |
| html_url                       | String        | &check;      |
| id                             | String        | &cross;      |
| initial_restore_id             | String        | &check;      |
| mysql_address                  | String        | &check;      |
| mysql_edge_address             | String        | &check;      |
| name                           | String        | &check;      |
| parent_branch                  | String        | &check;      |
| planetscale_region             | Region        | &check;      |
| production                     | Boolean       | &check;      |
| ready                          | Boolean       | &check;      |
| restore_checklist_completed_at | String        | &check;      |
| restored_from_branch           | RestoreBranch | &check;      |
| schema_last_updated_at         | String        | &check;      |
| shard_count                    | Int           | &check;      |
| sharded                        | Boolean       | &check;      |
| updated_at                     | String        | &check;      |

#### Actor
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| display_name | String   | &check;      |
| id           | String   | &check;      |

#### Region
| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| display_name        | String       | &check;      |
| enabled             | String       | &check;      |
| id                  | String       | &check;      |
| location            | String       | &check;      |
| provider            | String       | &check;      |
| public_ip_addresses | List<String> | &check;      |
| slug                | String       | &check;      |

#### RestoreBranch
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| created_at | String   | &check;      |
| deleted_at | String   | &check;      |
| id         | String   | &check;      |
| name       | String   | &check;      |
| updated_at | String   | &check;      |
