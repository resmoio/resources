---
description: ClickHouse Schema
---
clickhouse_schema
-----------------

| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| catalogName  | String   | &check;      |
| dbIdentifier | String   | &cross;      |
| name         | String   | &cross;      |
| owner        | String   | &check;      |

#### ClickHouseResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
