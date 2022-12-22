---
description: PlanetScale Database
---
planetscale_database
--------------------

| **Name**                               | **Type**   | **Nullable** |
| -------------------------------------- | ---------- | ------------ |
| allow_data_branching                   | Boolean    | &check;      |
| at_backup_restore_branches_limit       | Boolean    | &check;      |
| at_development_branch_limit            | Boolean    | &check;      |
| automatic_migrations                   | Boolean    | &check;      |
| branches_count                         | Int        | &check;      |
| branches_url                           | String     | &check;      |
| created_at                             | String     | &check;      |
| data_import                            | DataImport | &check;      |
| default_branch                         | String     | &check;      |
| default_branch_read_only_regions_count | Int        | &check;      |
| default_branch_shard_count             | Int        | &check;      |
| default_branch_table_count             | Int        | &check;      |
| development_branches_count             | Int        | &check;      |
| html_url                               | String     | &check;      |
| id                                     | String     | &cross;      |
| insights_raw_queries                   | Boolean    | &check;      |
| issues_count                           | Int        | &check;      |
| migration_framework                    | String     | &check;      |
| migration_table_name                   | String     | &check;      |
| multiple_admins_required_for_deletion  | Boolean    | &check;      |
| name                                   | String     | &check;      |
| notes                                  | String     | &check;      |
| organizationName                       | String     | &check;      |
| plan                                   | String     | &check;      |
| production_branch_web_console          | Boolean    | &check;      |
| production_branches_count              | Int        | &check;      |
| ready                                  | Boolean    | &check;      |
| region                                 | Region     | &check;      |
| require_approval_for_deploy            | Boolean    | &check;      |
| restrict_branch_region                 | Boolean    | &check;      |
| schema_last_updated_at                 | String     | &check;      |
| sharded                                | Boolean    | &check;      |
| state                                  | String     | &check;      |
| type                                   | String     | &check;      |
| updated_at                             | String     | &check;      |
| url                                    | String     | &check;      |

#### Actor
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| display_name | String   | &check;      |
| id           | String   | &check;      |

#### DataImport
| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| data_source         | Map<String,String> | &check;      |
| finished_at         | String             | &check;      |
| import_check_errors | String             | &check;      |
| started_at          | String             | &check;      |
| state               | String             | &check;      |

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
