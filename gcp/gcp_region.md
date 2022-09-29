---
description: Google Cloud Platform GCP Region
---
gcp_region
----------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| creationTimestamp | String       | &check;      |
| deprecated        | Deprecated   | &check;      |
| description       | String       | &check;      |
| id                | String       | &cross;      |
| kind              | String       | &cross;      |
| name              | String       | &check;      |
| project           | String       | &cross;      |
| selfLink          | String       | &check;      |
| status            | String       | &check;      |
| supportsPzs       | Boolean      | &check;      |
| zones             | List<String> | &check;      |

#### Deprecated
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| deleted     | String   | &check;      |
| deprecated  | String   | &check;      |
| obsolete    | String   | &check;      |
| replacement | String   | &check;      |
| state       | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### Quota
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| limit    | Double   | &check;      |
| metric   | String   | &check;      |
| owner    | String   | &check;      |
| usage    | Double   | &check;      |
