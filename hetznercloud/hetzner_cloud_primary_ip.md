---
description: Hetzner Cloud Primary IP
---
hetzner_cloud_primary_ip
------------------------

| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| assignee_id   | Long               | &check;      |
| assignee_type | String             | &check;      |
| auto_delete   | Boolean            | &check;      |
| blocked       | Boolean            | &check;      |
| created       | String             | &check;      |
| datacenter    | Datacenter         | &check;      |
| dns_ptr       | List<DnsPtr>       | &check;      |
| id            | Long               | &cross;      |
| ip            | String             | &check;      |
| labels        | Map<String,String> | &check;      |
| name          | String             | &check;      |
| protection    | Protection         | &check;      |
| type          | String             | &check;      |

#### Datacenter
| **Name**     | **Type**               | **Nullable** |
| ------------ | ---------------------- | ------------ |
| description  | String                 | &check;      |
| id           | Long                   | &check;      |
| location     | Datacenter.Location    | &check;      |
| name         | String                 | &check;      |
| server_types | Datacenter.ServerTypes | &check;      |

#### Datacenter.Location
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

#### Datacenter.ServerTypes
| **Name**                | **Type**   | **Nullable** |
| ----------------------- | ---------- | ------------ |
| available               | List<Long> | &check;      |
| available_for_migration | List<Long> | &check;      |
| supported               | List<Long> | &check;      |

#### DnsPtr
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dns_ptr  | String   | &check;      |
| ip       | String   | &check;      |

#### Protection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| delete   | Boolean  | &check;      |
