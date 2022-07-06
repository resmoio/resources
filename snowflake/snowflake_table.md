---
description: Snowflake Table
---
snowflake_table
---------------

| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| automatic_clustering         | String   | &check;      |
| change_tracking              | String   | &check;      |
| cluster_by                   | String   | &check;      |
| comment                      | String   | &check;      |
| created_on                   | String   | &check;      |
| database_name                | String   | &cross;      |
| is_external                  | String   | &check;      |
| kind                         | String   | &check;      |
| name                         | String   | &cross;      |
| owner                        | String   | &check;      |
| retention_time               | String   | &check;      |
| schema_name                  | String   | &cross;      |
| search_optimization          | String   | &check;      |
| search_optimization_bytes    | String   | &check;      |
| search_optimization_progress | String   | &check;      |
