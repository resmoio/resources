---
description: Google Cloud Platform SQL Backup
---
gcp_sql_backup
--------------

| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| backupKind                  | String                      | &check;      |
| description                 | String                      | &check;      |
| diskEncryptionConfiguration | DiskEncryptionConfiguration | &check;      |
| diskEncryptionStatus        | DiskEncryptionStatus        | &check;      |
| endTime                     | String                      | &check;      |
| enqueuedTime                | String                      | &check;      |
| error                       | OperationError              | &check;      |
| id                          | Long                        | &cross;      |
| instance                    | String                      | &check;      |
| kind                        | String                      | &check;      |
| location                    | String                      | &check;      |
| project                     | String                      | &cross;      |
| startTime                   | String                      | &check;      |
| status                      | String                      | &check;      |
| type                        | String                      | &check;      |
| windowStartTime             | String                      | &check;      |

#### DiskEncryptionConfiguration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| kind       | String   | &check;      |
| kmsKeyName | String   | &check;      |

#### DiskEncryptionStatus
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| kind              | String   | &check;      |
| kmsKeyVersionName | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### OperationError
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| kind     | String   | &check;      |
| message  | String   | &check;      |
