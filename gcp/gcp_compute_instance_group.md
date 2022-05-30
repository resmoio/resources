---
description: Google Cloud Platform Compute Instance Group
---
gcp_compute_instance_group
--------------------------

| **Name**          | **Type**        | **Nullable** |
| ----------------- | --------------- | ------------ |
| creationTimestamp | String          | &check;      |
| description       | String          | &check;      |
| id                | String          | &cross;      |
| kind              | String          | &check;      |
| name              | String          | &check;      |
| namedPorts        | List<NamedPort> | &check;      |
| network           | String          | &check;      |
| project           | String          | &cross;      |
| region            | String          | &check;      |
| size              | Int             | &check;      |
| subnetwork        | String          | &check;      |
| zone              | String          | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### NamedPort
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| port     | Int      | &check;      |
