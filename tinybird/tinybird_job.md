---
description: Tinybird Job
---
tinybird_job
------------

| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| createdAt  | String     | &check;      |
| datasource | DataSource | &check;      |
| id         | String     | &cross;      |
| jobUrl     | String     | &check;      |
| kind       | String     | &check;      |
| status     | String     | &check;      |
| updatedAt  | String     | &check;      |

#### DataSource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
