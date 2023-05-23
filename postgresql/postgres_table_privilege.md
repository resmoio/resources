---
description: PostgreSQL Table Privilege
---
postgres_table_privilege
------------------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| dbIdentifier  | String   | &check;      |
| grantable     | String   | &check;      |
| grantee       | String   | &check;      |
| grantor       | String   | &check;      |
| id            | String   | &cross;      |
| privilegeType | String   | &check;      |
| tableCatalog  | String   | &check;      |
| tableName     | String   | &check;      |
| tableSchema   | String   | &check;      |
| withHierarchy | String   | &check;      |
