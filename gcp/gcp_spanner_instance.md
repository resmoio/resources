---
description: Google Cloud Platform Spanner Instance
---
gcp_spanner_instance
--------------------

| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| config          | String             | &check;      |
| createTime      | String             | &check;      |
| displayName     | String             | &check;      |
| endpointUris    | List<String>       | &check;      |
| labels          | Map<String,String> | &check;      |
| name            | String             | &cross;      |
| nodeCount       | Int                | &check;      |
| processingUnits | Int                | &check;      |
| project         | String             | &cross;      |
| state           | String             | &check;      |
| updateTime      | String             | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
