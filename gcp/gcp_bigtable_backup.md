---
description: Google Cloud Platform BigTable Backup
---
gcp_bigtable_backup
-------------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| clusterId      | String         | &cross;      |
| encryptionInfo | EncryptionInfo | &check;      |
| endTime        | String         | &check;      |
| expireTime     | String         | &check;      |
| id             | String         | &cross;      |
| instanceId     | String         | &cross;      |
| project        | String         | &cross;      |
| sourceTableId  | String         | &check;      |
| startTime      | String         | &check;      |
| state          | String         | &check;      |

#### EncryptionInfo
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| kmsKeyVersion | String   | &check;      |
| status        | String   | &check;      |
| type          | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
