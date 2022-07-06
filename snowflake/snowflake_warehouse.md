---
description: Snowflake Warehouse
---
snowflake_warehouse
-------------------

| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| actives           | Int      | &check;      |
| auto_resume       | Boolean  | &check;      |
| auto_suspend      | Int      | &check;      |
| available         | String   | &check;      |
| comment           | String   | &check;      |
| created_on        | String   | &check;      |
| failed            | Int      | &check;      |
| is_current        | Boolean  | &check;      |
| is_default        | Boolean  | &check;      |
| max_cluster_count | Int      | &check;      |
| min_cluster_count | Int      | &check;      |
| name              | String   | &check;      |
| other             | String   | &check;      |
| owner             | String   | &check;      |
| pendings          | Int      | &check;      |
| provisioning      | String   | &check;      |
| queued            | Int      | &check;      |
| quiescing         | String   | &check;      |
| resource_monitor  | String   | &check;      |
| resumed_on        | String   | &check;      |
| running           | Int      | &check;      |
| scaling_policy    | String   | &check;      |
| started_clusters  | Int      | &check;      |
| state             | String   | &check;      |
| suspended         | Int      | &check;      |
| type              | String   | &check;      |
| updated_on        | String   | &check;      |
| uuid              | String   | &cross;      |
