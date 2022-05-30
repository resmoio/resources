---
description: Google Cloud Platform Compute Disk
---
gcp_compute_disk
----------------

| **Name**                           | **Type**              | **Nullable** |
| ---------------------------------- | --------------------- | ------------ |
| creationTimestamp                  | String                | &check;      |
| description                        | String                | &check;      |
| diskEncryptionKey                  | DiskEncryptionKey     | &check;      |
| guestOsFeatures                    | List<GuestOsFeatures> | &check;      |
| id                                 | String                | &cross;      |
| kind                               | String                | &cross;      |
| labels                             | Map<String,String>    | &check;      |
| lastAttachTimestamp                | String                | &check;      |
| lastDetachTimestamp                | String                | &check;      |
| licenseCodes                       | List<Long>            | &check;      |
| licenseCodesMemoizedSerializedSize | String                | &check;      |
| licenses                           | List<String>          | &check;      |
| locationHint                       | String                | &check;      |
| name                               | String                | &check;      |
| options                            | String                | &check;      |
| physicalBlockSizeBytes             | Long                  | &check;      |
| project                            | String                | &cross;      |
| provisionedIops                    | Long                  | &check;      |
| region                             | String                | &check;      |
| replicaZones                       | List<String>          | &check;      |
| resourcePolicies                   | List<String>          | &check;      |
| sizeGb                             | Long                  | &check;      |
| sourceDisk                         | String                | &check;      |
| sourceDiskId                       | String                | &check;      |
| sourceImage                        | String                | &check;      |
| sourceImageEncryptionKey           | DiskEncryptionKey     | &check;      |
| sourceImageId                      | String                | &check;      |
| sourceSnapshot                     | String                | &check;      |
| sourceSnapshotEncryptionKey        | DiskEncryptionKey     | &check;      |
| sourceSnapshotId                   | String                | &check;      |
| sourceStorageObject                | String                | &check;      |
| status                             | String                | &check;      |
| type                               | String                | &check;      |
| users                              | List<String>          | &check;      |
| zone                               | String                | &check;      |

#### DiskEncryptionKey
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| kmsKeyName           | String   | &check;      |
| kmsKeyServiceAccount | String   | &check;      |
| sha256               | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### GuestOsFeatures
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
