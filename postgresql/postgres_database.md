---
description: PostgreSQL Database
---
postgres_database
-----------------

| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| allowConnection | String   | &check;      |
| connectionLimit | String   | &check;      |
| dbIdentifier    | String   | &cross;      |
| name            | String   | &cross;      |
| template        | String   | &check;      |

#### PostgresResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
