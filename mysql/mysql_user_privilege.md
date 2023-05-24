---
description: MySQL User Privilege
---
mysql_user_privilege
--------------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| dbIdentifier  | String   | &cross;      |
| grantable     | String   | &check;      |
| grantee       | String   | &check;      |
| privilegeType | String   | &check;      |
| tableCatalog  | String   | &check;      |

#### MySqlResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
