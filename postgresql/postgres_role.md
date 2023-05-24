---
description: PostgreSQL Role
---
postgres_role
-------------

| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| byPassRls       | String   | &check;      |
| canLogin        | String   | &check;      |
| connectionLimit | String   | &check;      |
| createDatabase  | String   | &check;      |
| createRole      | String   | &check;      |
| dbIdentifier    | String   | &cross;      |
| inherit         | String   | &check;      |
| name            | String   | &cross;      |
| replication     | String   | &check;      |
| superRole       | String   | &check;      |

#### PostgresResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
