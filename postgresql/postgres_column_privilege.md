---
description: PostgreSQL Column Privilege
---
postgres_column_privilege
-------------------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| columnName    | String   | &check;      |
| dbIdentifier  | String   | &cross;      |
| grantable     | String   | &check;      |
| grantee       | String   | &check;      |
| grantor       | String   | &check;      |
| privilegeType | String   | &check;      |
| tableCatalog  | String   | &check;      |
| tableName     | String   | &check;      |
| tableSchema   | String   | &check;      |

#### PostgresResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
