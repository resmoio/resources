---
description: Google Cloud Platform Spanner Database
---
gcp_spanner_database
--------------------

| **Name**               | **Type**             | **Nullable** |
| ---------------------- | -------------------- | ------------ |
| createTime             | String               | &check;      |
| databaseDialect        | String               | &check;      |
| defaultLeader          | String               | &check;      |
| encryptionConfig       | EncryptionConfig     | &check;      |
| encryptionInfo         | List<EncryptionInfo> | &check;      |
| name                   | String               | &cross;      |
| project                | String               | &cross;      |
| restoreInfo            | RestoreInfo          | &check;      |
| state                  | String               | &check;      |
| versionRetentionPeriod | String               | &check;      |

#### EncryptionConfig
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| kmsKeyName | String   | &check;      |

#### EncryptionInfo
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| encryptionType | String   | &check;      |
| kmsKeyVersion  | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### RestoreInfo
| **Name**   | **Type**               | **Nullable** |
| ---------- | ---------------------- | ------------ |
| backupInfo | RestoreInfo.BackupInfo | &check;      |
| sourceType | String                 | &check;      |

#### RestoreInfo.BackupInfo
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| backup         | String   | &check;      |
| createTime     | String   | &check;      |
| sourceDatabase | String   | &check;      |
| versionTime    | String   | &check;      |
