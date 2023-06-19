---
description: Hetzner Cloud Floating IP
---
hetzner_cloud_floating_ip
-------------------------

| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| blocked       | Boolean            | &check;      |
| created       | String             | &check;      |
| description   | String             | &check;      |
| dns_ptr       | List<DnsPtr>       | &check;      |
| home_location | HomeLocation       | &check;      |
| id            | Long               | &check;      |
| ip            | String             | &check;      |
| labels        | Map<String,String> | &check;      |
| name          | String             | &check;      |
| protection    | Protection         | &check;      |
| server        | Long               | &check;      |
| type          | String             | &check;      |

#### DnsPtr
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dns_ptr  | String   | &check;      |
| ip       | String   | &check;      |

#### HomeLocation
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
