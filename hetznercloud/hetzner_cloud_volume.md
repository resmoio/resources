---
description: Hetzner Cloud Volume
---
hetzner_cloud_volume
--------------------

| **Name**     | **Type**           | **Nullable** |
| ------------ | ------------------ | ------------ |
| created      | String             | &check;      |
| format       | String             | &check;      |
| id           | Long               | &cross;      |
| labels       | Map<String,String> | &check;      |
| linux_device | String             | &check;      |
| location     | Location           | &check;      |
| name         | String             | &check;      |
| protection   | Protection         | &check;      |
| server       | Long               | &check;      |
| size         | Long               | &check;      |
| status       | String             | &check;      |

#### Location
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| city         | String   | &check;      |
| country      | String   | &check;      |
| description  | String   | &check;      |
| id           | Long     | &check;      |
| latitude     | Double   | &check;      |
| longitude    | Double   | &check;      |
| name         | String   | &check;      |
| network_zone | String   | &check;      |

#### Protection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| delete   | Boolean  | &check;      |
