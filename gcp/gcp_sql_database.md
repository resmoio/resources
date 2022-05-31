---
description: Google Cloud Platform SQL Database
---
gcp_sql_database
----------------

| **Name**                 | **Type**                 | **Nullable** |
| ------------------------ | ------------------------ | ------------ |
| charset                  | String                   | &check;      |
| collation                | String                   | &check;      |
| instance                 | String                   | &check;      |
| kind                     | String                   | &check;      |
| name                     | String                   | &cross;      |
| project                  | String                   | &cross;      |
| sqlserverDatabaseDetails | SqlServerDatabaseDetails | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### SqlServerDatabaseDetails
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| compatibilityLevel | Int      | &check;      |
| recoveryModel      | String   | &check;      |
