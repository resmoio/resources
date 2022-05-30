---
description: Google Cloud Platform Compute SSL Policy
---
gcp_compute_ssl_policy
----------------------

| **Name**          | **Type**       | **Nullable** |
| ----------------- | -------------- | ------------ |
| creationTimestamp | String         | &check;      |
| customFeatures    | List<String>   | &check;      |
| description       | String         | &check;      |
| enabledFeatures   | List<String>   | &check;      |
| id                | String         | &cross;      |
| kind              | String         | &check;      |
| minTlsVersion     | String         | &check;      |
| name              | String         | &check;      |
| profile           | String         | &check;      |
| project           | String         | &cross;      |
| warnings          | List<Warnings> | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### Warnings
| **Name** | **Type**            | **Nullable** |
| -------- | ------------------- | ------------ |
| code     | String              | &check;      |
| data     | List<Warnings.Data> | &check;      |
| message  | String              | &check;      |

#### Warnings.Data
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| value    | String   | &check;      |
