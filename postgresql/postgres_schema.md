---
description: PostgreSQL Schema
---
postgres_schema
---------------

| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| catalogName  | String   | &check;      |
| dbIdentifier | String   | &cross;      |
| name         | String   | &cross;      |
| owner        | String   | &check;      |

#### PostgresResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
