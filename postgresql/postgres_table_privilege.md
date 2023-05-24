---
description: PostgreSQL Table Privilege
---
postgres_table_privilege
------------------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| dbIdentifier  | String   | &cross;      |
| grantable     | String   | &check;      |
| grantee       | String   | &check;      |
| grantor       | String   | &check;      |
| privilegeType | String   | &check;      |
| tableCatalog  | String   | &check;      |
| tableName     | String   | &check;      |
| tableSchema   | String   | &check;      |
| withHierarchy | String   | &check;      |

#### PostgresResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
