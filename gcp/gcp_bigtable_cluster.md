---
description: Google Cloud Platform BigTable Cluster
---
gcp_bigtable_cluster
--------------------

| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| autoscalingCpuPercentageTarget | Int      | &check;      |
| autoscalingMaxServeNodes       | Int      | &check;      |
| autoscalingMinServeNodes       | Int      | &check;      |
| id                             | String   | &cross;      |
| instanceId                     | String   | &check;      |
| kmsKeyName                     | String   | &check;      |
| project                        | String   | &cross;      |
| serveNodes                     | Int      | &check;      |
| state                          | String   | &check;      |
| storageType                    | String   | &check;      |
| zone                           | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
