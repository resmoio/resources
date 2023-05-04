---
description: PostgreSQL Column Privilege
---
postgres_column_privilege
-------------------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| columnName    | String   | &check;      |
| dbEndpoint    | String   | &check;      |
| grantable     | String   | &check;      |
| grantee       | String   | &check;      |
| grantor       | String   | &check;      |
| id            | String   | &cross;      |
| privilegeType | String   | &check;      |
| tableCatalog  | String   | &check;      |
| tableName     | String   | &check;      |
| tableSchema   | String   | &check;      |
