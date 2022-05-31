---
description: Google Cloud Platform BigQuery Table
---
gcp_bigquery_table
------------------

| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| creationTime            | Long                    | &check;      |
| definition              | TableDefinition         | &check;      |
| description             | String                  | &check;      |
| encryptionConfiguration | EncryptionConfiguration | &check;      |
| expirationTime          | Long                    | &check;      |
| friendlyName            | String                  | &check;      |
| generatedId             | String                  | &check;      |
| labels                  | Map<String,String>      | &check;      |
| lastModifiedTime        | Long                    | &check;      |
| project                 | String                  | &cross;      |
| requirePartitionFilter  | Boolean                 | &check;      |
| tableId                 | TableId                 | &cross;      |

#### EncryptionConfiguration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| kmsKeyName | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### TableDefinition
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| schema   | JSON     | &check;      |
| type     | String   | &check;      |

#### TableId
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dataset  | String   | &check;      |
| project  | String   | &check;      |
| table    | String   | &check;      |
