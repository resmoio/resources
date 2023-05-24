---
description: PostgreSQL Extension
---
postgres_extension
------------------

| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| dbIdentifier | String   | &cross;      |
| name         | String   | &cross;      |
| owner        | String   | &check;      |
| relocatable  | String   | &check;      |
| version      | String   | &check;      |

#### PostgresResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
