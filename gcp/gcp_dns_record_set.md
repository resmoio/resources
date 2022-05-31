---
description: Google Cloud Platform DNS Record Set
---
gcp_dns_record_set
------------------

| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| name     | String       | &cross;      |
| project  | String       | &cross;      |
| rrdatas  | List<String> | &check;      |
| ttl      | Int          | &check;      |
| type     | String       | &check;      |
| zone     | String       | &cross;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
