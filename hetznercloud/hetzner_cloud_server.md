---
description: Hetzner Cloud Server
---
hetzner_cloud_server
--------------------

| **Name**          | **Type**           | **Nullable** |
| ----------------- | ------------------ | ------------ |
| backup_window     | String             | &check;      |
| created           | String             | &check;      |
| datacenter        | Datacenter         | &check;      |
| id                | Long               | &cross;      |
| image             | Image              | &check;      |
| iso               | Iso                | &check;      |
| labels            | Map<String,String> | &check;      |
| load_balancers    | List<Long>         | &check;      |
| locked            | Boolean            | &check;      |
| name              | String             | &check;      |
| outgoing_traffic  | Long               | &check;      |
| placement_group   | PlacementGroup     | &check;      |
| primary_disk_size | Long               | &check;      |
| private_net       | List<PrivateNet>   | &check;      |
| protection        | Protection         | &check;      |
| public_net        | PublicNet          | &check;      |
| rescue_enabled    | Boolean            | &check;      |
| server_type       | ServerType         | &check;      |
| status            | String             | &check;      |
| volumes           | List<Long>         | &check;      |

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
| **Name**  | **Type**   | **Nullable** |
| --------- | ---------- | ------------ |
| supported | List<Long> | &check;      |

#### Image
| **Name**     | **Type**           | **Nullable** |
| ------------ | ------------------ | ------------ |
| architecture | String             | &check;      |
| bound_to     | Long               | &check;      |
| created      | String             | &check;      |
| created_from | Image.CreatedFrom  | &check;      |
| deleted      | String             | &check;      |
| deprecated   | String             | &check;      |
| description  | String             | &check;      |
| disk_size    | Long               | &check;      |
| id           | Long               | &check;      |
| image_size   | Double             | &check;      |
| labels       | Map<String,String> | &check;      |
| name         | String             | &check;      |
| os_flavor    | String             | &check;      |
| os_version   | String             | &check;      |
| protection   | Image.Protection   | &check;      |
| rapid_deploy | Boolean            | &check;      |
| status       | String             | &check;      |
| type         | String             | &check;      |

#### Image.CreatedFrom
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |
| name     | String   | &check;      |

#### Image.Protection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| delete   | Boolean  | &check;      |

#### Iso
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| architecture | String   | &check;      |
| deprecated   | String   | &check;      |
| description  | String   | &check;      |
| id           | Long     | &check;      |
| name         | String   | &check;      |
| type         | String   | &check;      |

#### PlacementGroup
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| created  | String             | &check;      |
| id       | Long               | &check;      |
| labels   | Map<String,String> | &check;      |
| name     | String             | &check;      |
| servers  | List<Long>         | &check;      |
| type     | String             | &check;      |

#### PrivateNet
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| alias_ips   | List<String> | &check;      |
| ip          | String       | &check;      |
| mac_address | String       | &check;      |
| network     | Long         | &check;      |

#### Protection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| delete   | Boolean  | &check;      |
| rebuild  | Boolean  | &check;      |

#### PublicNet
| **Name**     | **Type**                 | **Nullable** |
| ------------ | ------------------------ | ------------ |
| firewalls    | List<PublicNet.Firewall> | &check;      |
| floating_ips | List<Long>               | &check;      |
| ipv4         | PublicNet.Ipv4           | &check;      |
| ipv6         | PublicNet.Ipv6           | &check;      |

#### PublicNet.Firewall
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |
| status   | String   | &check;      |

#### PublicNet.Ipv4
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| blocked  | Boolean  | &check;      |
| dns_ptr  | String   | &check;      |
| id       | Long     | &check;      |
| ip       | String   | &check;      |

#### PublicNet.Ipv6
| **Name** | **Type**                    | **Nullable** |
| -------- | --------------------------- | ------------ |
| blocked  | Boolean                     | &check;      |
| dns_ptr  | List<PublicNet.Ipv6.DnsPtr> | &check;      |
| id       | Long                        | &check;      |
| ip       | String                      | &check;      |

#### PublicNet.Ipv6.DnsPtr
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dns_ptr  | String   | &check;      |
| ip       | String   | &check;      |

#### ServerType
| **Name**     | **Type**               | **Nullable** |
| ------------ | ---------------------- | ------------ |
| cores        | Long                   | &check;      |
| cpu_type     | String                 | &check;      |
| deprecated   | Boolean                | &check;      |
| description  | String                 | &check;      |
| disk         | Long                   | &check;      |
| id           | Long                   | &check;      |
| memory       | Long                   | &check;      |
| name         | String                 | &check;      |
| prices       | List<ServerType.Price> | &check;      |
| storage_type | String                 | &check;      |

#### ServerType.Price
| **Name**      | **Type**                      | **Nullable** |
| ------------- | ----------------------------- | ------------ |
| location      | String                        | &check;      |
| price_hourly  | ServerType.Price.PriceHourly  | &check;      |
| price_monthly | ServerType.Price.PriceMonthly | &check;      |

#### ServerType.Price.PriceHourly
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gross    | String   | &check;      |
| net      | String   | &check;      |

#### ServerType.Price.PriceMonthly
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gross    | String   | &check;      |
| net      | String   | &check;      |
