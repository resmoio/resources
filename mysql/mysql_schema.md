---
description: MySQL Schema
---
mysql_schema
------------

| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| catalogName             | String   | &check;      |
| dbIdentifier            | String   | &cross;      |
| defaultCharacterSetName | String   | &check;      |
| defaultEncryption       | String   | &check;      |
| name                    | String   | &cross;      |

#### MySqlResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
