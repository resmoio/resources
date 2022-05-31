---
description: Google Cloud Platform AppEngine Instance
---
gcp_appengine_instance
----------------------

| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| appEngineRelease | String   | &check;      |
| availability     | String   | &check;      |
| averageLatency   | Int      | &check;      |
| errors           | Int      | &check;      |
| id               | String   | &cross;      |
| memoryUsage      | String   | &check;      |
| name             | String   | &cross;      |
| project          | String   | &cross;      |
| qps              | Number   | &check;      |
| requests         | Int      | &check;      |
| startTime        | String   | &check;      |
| vmDebugEnabled   | Boolean  | &check;      |
| vmId             | String   | &check;      |
| vmIp             | String   | &check;      |
| vmLiveness       | String   | &check;      |
| vmName           | String   | &check;      |
| vmStatus         | String   | &check;      |
| vmZoneName       | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
