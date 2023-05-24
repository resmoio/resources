---
description: ClickHouse User
---
clickhouse_user
---------------

| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| dbIdentifier       | String       | &cross;      |
| defaultRolesAll    | String       | &check;      |
| defaultRolesExcept | List<String> | &check;      |
| defaultRolesList   | List<String> | &check;      |
| granteesAny        | String       | &check;      |
| granteesExcept     | List<String> | &check;      |
| granteesList       | List<String> | &check;      |
| hostIp             | List<String> | &check;      |
| hostNames          | List<String> | &check;      |
| id                 | String       | &cross;      |
| name               | String       | &check;      |
| storage            | String       | &check;      |

#### ClickHouseResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
