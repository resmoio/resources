---
description: Google Cloud Platform AppEngine Service
---
gcp_appengine_service
---------------------

| **Name**        | **Type**        | **Nullable** |
| --------------- | --------------- | ------------ |
| id              | String          | &cross;      |
| name            | String          | &cross;      |
| networkSettings | NetworkSettings | &check;      |
| project         | String          | &cross;      |
| split           | TrafficSplit    | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### NetworkSettings
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| ingressTrafficAllowed | String   | &check;      |

#### TrafficSplit
| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| allocations | Map<String,Double> | &check;      |
| shardBy     | String             | &check;      |
