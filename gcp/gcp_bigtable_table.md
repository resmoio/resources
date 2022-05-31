---
description: Google Cloud Platform BigTable Table
---
gcp_bigtable_table
------------------

| **Name**                     | **Type**           | **Nullable** |
| ---------------------------- | ------------------ | ------------ |
| columnFamilies               | List<ColumnFamily> | &check;      |
| id                           | String             | &cross;      |
| instanceId                   | String             | &check;      |
| project                      | String             | &cross;      |
| replicationStatesByClusterId | Map<String,String> | &check;      |

#### ColumnFamily
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| rule     | JSON     | &cross;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
