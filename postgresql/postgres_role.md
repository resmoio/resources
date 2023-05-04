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
| dbEndpoint      | String   | &check;      |
| id              | String   | &cross;      |
| inherit         | String   | &check;      |
| name            | String   | &check;      |
| replication     | String   | &check;      |
| superRole       | String   | &check;      |
