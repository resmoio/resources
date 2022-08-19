---
description: Amazon Web Services Glue Catalog Table
---
aws_glue_catalog_table
----------------------

| **Name**                      | **Type**           | **Nullable** |
| ----------------------------- | ------------------ | ------------ |
| accountId                     | String             | &cross;      |
| accountName                   | String             | &check;      |
| catalogId                     | String             | &check;      |
| createTime                    | String             | &check;      |
| createdBy                     | String             | &check;      |
| databaseName                  | String             | &cross;      |
| description                   | String             | &check;      |
| isRegisteredWithLakeFormation | Boolean            | &check;      |
| lastAccessTime                | String             | &check;      |
| lastAnalyzedTime              | String             | &check;      |
| name                          | String             | &cross;      |
| owner                         | String             | &check;      |
| parameters                    | Map<String,String> | &check;      |
| partitionKeys                 | List<Column>       | &check;      |
| region                        | String             | &cross;      |
| retention                     | Int                | &check;      |
| storageDescriptor             | StorageDescriptor  | &check;      |
| tableType                     | String             | &check;      |
| targetTable                   | TableIdentifier    | &check;      |
| updateTime                    | String             | &check;      |
| versionId                     | String             | &check;      |
| viewExpandedText              | String             | &check;      |
| viewOriginalText              | String             | &check;      |

#### Column
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| comment    | String             | &check;      |
| name       | String             | &check;      |
| parameters | Map<String,String> | &check;      |
| type       | String             | &check;      |

#### Order
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| column    | String   | &check;      |
| sortOrder | Int      | &check;      |

#### SchemaId
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| registryName | String   | &check;      |
| schemaArn    | String   | &check;      |
| schemaName   | String   | &check;      |

#### SchemaReference
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| schemaId            | SchemaId | &check;      |
| schemaVersionId     | String   | &check;      |
| schemaVersionNumber | Long     | &check;      |

#### SerDeInfo
| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| name                 | String             | &check;      |
| parameters           | Map<String,String> | &check;      |
| serializationLibrary | String             | &check;      |

#### SkewedInfo
| **Name**                      | **Type**           | **Nullable** |
| ----------------------------- | ------------------ | ------------ |
| skewedColumnNames             | List<String>       | &check;      |
| skewedColumnValueLocationMaps | Map<String,String> | &check;      |
| skewedColumnValues            | List<String>       | &check;      |

#### StorageDescriptor
| **Name**               | **Type**           | **Nullable** |
| ---------------------- | ------------------ | ------------ |
| additionalLocations    | List<String>       | &check;      |
| bucketColumns          | List<String>       | &check;      |
| columns                | List<Column>       | &check;      |
| compressed             | Boolean            | &check;      |
| inputFormat            | String             | &check;      |
| location               | String             | &check;      |
| numberOfBuckets        | Int                | &check;      |
| outputFormat           | String             | &check;      |
| parameters             | Map<String,String> | &check;      |
| schemaReference        | SchemaReference    | &check;      |
| serdeInfo              | SerDeInfo          | &check;      |
| skewedInfo             | SkewedInfo         | &check;      |
| sortColumns            | List<Order>        | &check;      |
| storedAsSubDirectories | Boolean            | &check;      |

#### TableIdentifier
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| catalogId    | String   | &check;      |
| databaseName | String   | &check;      |
| name         | String   | &check;      |
