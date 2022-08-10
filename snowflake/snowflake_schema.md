---
description: Snowflake Schema
---
snowflake_schema
----------------

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| comment        | String   | &check;      |
| created_on     | String   | &check;      |
| database_name  | String   | &cross;      |
| is_current     | Boolean  | &check;      |
| is_default     | Boolean  | &check;      |
| name           | String   | &cross;      |
| options        | String   | &check;      |
| owner          | String   | &check;      |
| retention_time | String   | &check;      |
