---
description: Google Cloud Platform Spanner Instance Config
---
gcp_spanner_instance_config
---------------------------

| **Name**      | **Type**          | **Nullable** |
| ------------- | ----------------- | ------------ |
| displayName   | String            | &check;      |
| leaderOptions | List<String>      | &check;      |
| name          | String            | &cross;      |
| project       | String            | &cross;      |
| replicas      | List<ReplicaInfo> | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### ReplicaInfo
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| defaultLeaderLocation | Boolean  | &check;      |
| location              | String   | &check;      |
| type                  | String   | &check;      |
