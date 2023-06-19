---
description: Hetzner Cloud Datacenter
---
hetzner_cloud_datacenter
------------------------

| **Name**     | **Type**         | **Nullable** |
| ------------ | ---------------- | ------------ |
| description  | String           | &check;      |
| id           | Long             | &cross;      |
| location     | Location         | &check;      |
| name         | String           | &check;      |
| server_types | Map<String,List> | &check;      |

#### Location
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| city         | String   | &check;      |
| county       | String   | &check;      |
| description  | String   | &check;      |
| id           | Long     | &cross;      |
| latitude     | Double   | &check;      |
| longitude    | Double   | &check;      |
| name         | String   | &check;      |
| network_zone | String   | &check;      |
