---
description: Google Cloud Platform BigQuery Dataset
---
gcp_bigquery_dataset
--------------------

| **Name**                       | **Type**                | **Nullable** |
| ------------------------------ | ----------------------- | ------------ |
| acl                            | List<Acl>               | &check;      |
| creationTime                   | Long                    | &check;      |
| datasetId                      | DatasetId               | &cross;      |
| defaultEncryptionConfiguration | EncryptionConfiguration | &check;      |
| defaultPartitionExpirationMs   | Long                    | &check;      |
| defaultTableLifetime           | Long                    | &check;      |
| description                    | String                  | &check;      |
| friendlyName                   | String                  | &check;      |
| generatedId                    | String                  | &check;      |
| labels                         | Map<String,String>      | &check;      |
| lastModified                   | Long                    | &check;      |
| location                       | String                  | &check;      |
| project                        | String                  | &cross;      |

#### Acl
| **Name** | **Type**   | **Nullable** |
| -------- | ---------- | ------------ |
| entity   | Acl.Entity | &check;      |
| role     | String     | &check;      |

#### Acl.Entity
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| entityIdentifier | String   | &check;      |
| type             | String   | &check;      |

#### DatasetId
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dataset  | String   | &check;      |
| project  | String   | &check;      |

#### EncryptionConfiguration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| kmsKeyName | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
