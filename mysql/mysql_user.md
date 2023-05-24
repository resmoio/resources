---
description: MySQL User
---
mysql_user
----------

| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| alterPrivilege            | String   | &check;      |
| alterRoutinePrivilege     | String   | &check;      |
| createPrivilege           | String   | &check;      |
| createRolePrivilege       | String   | &check;      |
| createRoutinePrivilege    | String   | &check;      |
| createTablespacePrivilege | String   | &check;      |
| createTmpTablesPrivilege  | String   | &check;      |
| createUserPrivilege       | String   | &check;      |
| createViewPrivilege       | String   | &check;      |
| dbIdentifier              | String   | &cross;      |
| deletePrivilege           | String   | &check;      |
| dropPrivilege             | String   | &check;      |
| dropRolePrivilege         | String   | &check;      |
| eventPrivilege            | String   | &check;      |
| executePrivilege          | String   | &check;      |
| filePrivilege             | String   | &check;      |
| grantPrivilege            | String   | &check;      |
| host                      | String   | &check;      |
| indexPrivilege            | String   | &check;      |
| insertPrivilege           | String   | &check;      |
| lockTablesPrivilege       | String   | &check;      |
| passwordExpired           | String   | &check;      |
| processPrivilege          | String   | &check;      |
| referencesPrivilege       | String   | &check;      |
| reloadPrivilege           | String   | &check;      |
| replClientPrivilege       | String   | &check;      |
| replSlavePrivilege        | String   | &check;      |
| selectPrivilege           | String   | &check;      |
| showDatabasePrivilege     | String   | &check;      |
| showViewPrivilege         | String   | &check;      |
| shutdownPrivilege         | String   | &check;      |
| sslType                   | String   | &check;      |
| superPrivilege            | String   | &check;      |
| triggerPrivilege          | String   | &check;      |
| updatePrivilege           | String   | &check;      |
| user                      | String   | &cross;      |

#### MySqlResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
