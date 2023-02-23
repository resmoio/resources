---
description: Tinybird Datasource
---
tinybird_datasource
-------------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| cluster            | String             | &check;      |
| columns            | List<Column>       | &check;      |
| createdAt          | String             | &check;      |
| description        | String             | &check;      |
| engine             | Engine             | &check;      |
| headers            | Map<String,String> | &check;      |
| id                 | String             | &cross;      |
| name               | String             | &check;      |
| newColumnsDetected | Map<String,Column> | &check;      |
| project            | String             | &check;      |
| quarantineRows     | Int                | &check;      |
| replicated         | Boolean            | &check;      |
| sharedWith         | List<String>       | &check;      |
| statistics         | Statistics         | &check;      |
| type               | String             | &check;      |
| updatedAt          | String             | &check;      |
| usedBy             | List<Map>          | &check;      |
| version            | Int                | &check;      |

#### Column
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| codec          | String   | &check;      |
| defaultValue   | String   | &check;      |
| jsonpath       | String   | &check;      |
| name           | String   | &check;      |
| normalizedName | String   | &check;      |
| nullable       | Boolean  | &check;      |
| type           | String   | &check;      |

#### Engine
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| engine             | String   | &check;      |
| enginePartitionKey | String   | &check;      |
| enginePrimaryKey   | String   | &check;      |
| engineSortingKey   | String   | &check;      |

#### Statistics
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| bytes    | Long     | &check;      |
| rowCount | Long     | &check;      |
