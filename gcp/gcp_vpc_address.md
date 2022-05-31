---
description: Google Cloud Platform VPC Address
---
gcp_vpc_address
---------------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| address           | String       | &check;      |
| addressType       | String       | &check;      |
| creationTimestamp | String       | &check;      |
| description       | String       | &check;      |
| id                | String       | &cross;      |
| ipVersion         | String       | &check;      |
| kind              | String       | &check;      |
| name              | String       | &check;      |
| network           | String       | &check;      |
| networkTier       | String       | &check;      |
| prefixLength      | String       | &check;      |
| project           | String       | &cross;      |
| purpose           | String       | &check;      |
| region            | String       | &check;      |
| status            | String       | &check;      |
| subnetwork        | String       | &check;      |
| users             | List<String> | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
