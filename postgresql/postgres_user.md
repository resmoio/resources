---
description: PostgreSQL User
---
postgres_user
-------------

| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| byPassRls         | String   | &check;      |
| canCreateDatabase | String   | &check;      |
| config            | String   | &check;      |
| dbIdentifier      | String   | &cross;      |
| name              | String   | &cross;      |
| repl              | String   | &check;      |
| superUser         | String   | &check;      |

#### PostgresResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
