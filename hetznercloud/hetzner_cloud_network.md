---
description: Hetzner Cloud Network
---
hetzner_cloud_network
---------------------

| **Name**       | **Type**           | **Nullable** |
| -------------- | ------------------ | ------------ |
| created        | String             | &check;      |
| id             | Long               | &cross;      |
| ip_range       | String             | &check;      |
| labels         | Map<String,String> | &check;      |
| load_balancers | List<Long>         | &check;      |
| name           | String             | &check;      |
| protection     | Protection         | &check;      |
| routes         | List<Route>        | &check;      |
| servers        | List<Long>         | &check;      |
| subnets        | List<Subnet>       | &check;      |

#### Protection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| delete   | Boolean  | &check;      |

#### Route
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| destination | String   | &check;      |
| gateway     | String   | &check;      |

#### Subnet
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| gateway      | String   | &check;      |
| ip_range     | String   | &check;      |
| network_zone | String   | &check;      |
| type         | String   | &check;      |
