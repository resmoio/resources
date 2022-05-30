---
description: Google Cloud Platform PUB/SUB Topic
---
gcp_pubsub_topic
----------------

| **Name**                 | **Type**             | **Nullable** |
| ------------------------ | -------------------- | ------------ |
| kmsKeyName               | String               | &check;      |
| labels                   | Map<String,String>   | &check;      |
| messageRetentionDuration | String               | &check;      |
| messageStoragePolicy     | MessageStoragePolicy | &check;      |
| name                     | String               | &cross;      |
| project                  | String               | &cross;      |
| satisfiesPzs             | Boolean              | &check;      |
| schemaSettings           | SchemaSettings       | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### MessageStoragePolicy
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| allowedPersistenceRegions | List<String> | &check;      |

#### SchemaSettings
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| encoding | String   | &check;      |
| schema   | String   | &check;      |
