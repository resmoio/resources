---
description: Tinybird Pipe
---
tinybird_pipe
-------------

| **Name**    | **Type**   | **Nullable** |
| ----------- | ---------- | ------------ |
| createdAt   | String     | &check;      |
| description | String     | &check;      |
| endpoint    | String     | &check;      |
| id          | String     | &cross;      |
| name        | String     | &check;      |
| nodes       | List<Node> | &check;      |
| parent      | String     | &check;      |
| updatedAt   | String     | &check;      |
| url         | String     | &check;      |

#### Node
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| cluster         | String   | &check;      |
| createdAt       | String   | &check;      |
| description     | String   | &check;      |
| id              | String   | &check;      |
| ignoreSqlErrors | Boolean  | &check;      |
| materialized    | String   | &check;      |
| name            | String   | &check;      |
| project         | String   | &check;      |
| result          | String   | &check;      |
| sql             | String   | &check;      |
| updatedAt       | String   | &check;      |
| version         | Int      | &check;      |
