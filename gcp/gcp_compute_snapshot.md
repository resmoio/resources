---
description: Google Cloud Platform Compute Snapshot
---
gcp_compute_snapshot
--------------------

| **Name**                | **Type**              | **Nullable** |
| ----------------------- | --------------------- | ------------ |
| autoCreated             | Boolean               | &check;      |
| chainName               | String                | &check;      |
| creationTimestamp       | String                | &check;      |
| description             | String                | &check;      |
| diskSizeGb              | Long                  | &check;      |
| id                      | String                | &cross;      |
| kind                    | String                | &check;      |
| labels                  | Map<String,String>    | &check;      |
| licenseCodes            | List<Long>            | &check;      |
| licenses                | List<String>          | &check;      |
| name                    | String                | &check;      |
| project                 | String                | &cross;      |
| snapshotEncryptionKey   | CustomerEncryptionKey | &check;      |
| sourceDisk              | String                | &check;      |
| sourceDiskEncryptionKey | CustomerEncryptionKey | &check;      |
| sourceDiskId            | String                | &check;      |
| status                  | String                | &check;      |
| storageBytesStatus      | String                | &check;      |
| storageLocations        | List<String>          | &check;      |

#### CustomerEncryptionKey
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| kmsKeyName           | String   | &check;      |
| kmsKeyServiceAccount | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
