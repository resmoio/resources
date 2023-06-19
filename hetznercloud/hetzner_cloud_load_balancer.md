---
description: Hetzner Cloud Load Balancer
---
hetzner_cloud_load_balancer
---------------------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| algorithm          | Algorithm          | &check;      |
| created            | String             | &check;      |
| id                 | Long               | &cross;      |
| included_traffic   | Long               | &check;      |
| ingoing_traffic    | Long               | &check;      |
| labels             | Map<String,String> | &check;      |
| load_balancer_type | LoadBalancerType   | &check;      |
| location           | Location           | &check;      |
| name               | String             | &check;      |
| outgoing_traffic   | Long               | &check;      |
| private_net        | List<PrivateNet>   | &check;      |
| protection         | Protection         | &check;      |
| public_net         | PublicNet          | &check;      |
| services           | List<Service>      | &check;      |
| targets            | List<Target>       | &check;      |

#### Algorithm
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### LoadBalancerType
| **Name**                  | **Type**                     | **Nullable** |
| ------------------------- | ---------------------------- | ------------ |
| deprecated                | String                       | &check;      |
| description               | String                       | &check;      |
| id                        | Long                         | &check;      |
| max_assigned_certificates | Long                         | &check;      |
| max_connections           | Long                         | &check;      |
| max_services              | Long                         | &check;      |
| max_targets               | Long                         | &check;      |
| name                      | String                       | &check;      |
| prices                    | List<LoadBalancerType.Price> | &check;      |

#### LoadBalancerType.Price
| **Name**      | **Type**                            | **Nullable** |
| ------------- | ----------------------------------- | ------------ |
| location      | String                              | &check;      |
| price_hourly  | LoadBalancerType.Price.PriceHourly  | &check;      |
| price_monthly | LoadBalancerType.Price.PriceMonthly | &check;      |

#### LoadBalancerType.Price.PriceHourly
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gross    | String   | &check;      |
| net      | String   | &check;      |

#### LoadBalancerType.Price.PriceMonthly
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gross    | String   | &check;      |
| net      | String   | &check;      |

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

#### PrivateNet
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| ip       | String   | &check;      |
| network  | Long     | &check;      |

#### Protection
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| delete   | Boolean  | &check;      |

#### PublicNet
| **Name** | **Type**       | **Nullable** |
| -------- | -------------- | ------------ |
| enabled  | Boolean        | &check;      |
| ipv4     | PublicNet.Ipv4 | &check;      |
| ipv6     | PublicNet.Ipv6 | &check;      |

#### PublicNet.Ipv4
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dns_ptr  | String   | &check;      |
| ip       | String   | &check;      |

#### PublicNet.Ipv6
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| dns_ptr  | String   | &check;      |
| ip       | String   | &check;      |

#### Service
| **Name**         | **Type**            | **Nullable** |
| ---------------- | ------------------- | ------------ |
| destination_port | Long                | &check;      |
| health_check     | Service.HealthCheck | &check;      |
| http             | Service.Http        | &check;      |
| listen_port      | Long                | &check;      |
| protocol         | String              | &check;      |
| proxyprotocol    | Boolean             | &check;      |

#### Service.HealthCheck
| **Name** | **Type**                 | **Nullable** |
| -------- | ------------------------ | ------------ |
| http     | Service.HealthCheck.Http | &check;      |
| interval | Long                     | &check;      |
| port     | Long                     | &check;      |
| protocol | String                   | &check;      |
| retries  | Long                     | &check;      |
| timeout  | Long                     | &check;      |

#### Service.HealthCheck.Http
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| domain       | String       | &check;      |
| path         | String       | &check;      |
| response     | String       | &check;      |
| status_codes | List<String> | &check;      |
| tls          | Boolean      | &check;      |

#### Service.Http
| **Name**        | **Type**   | **Nullable** |
| --------------- | ---------- | ------------ |
| certificates    | List<Long> | &check;      |
| cookie_lifetime | Long       | &check;      |
| cookie_name     | String     | &check;      |
| redirect_http   | Boolean    | &check;      |
| sticky_sessions | Boolean    | &check;      |

#### Target
| **Name**       | **Type**                  | **Nullable** |
| -------------- | ------------------------- | ------------ |
| health_status  | List<Target.HealthStatus> | &check;      |
| ip             | Target.Ip                 | &check;      |
| label_selector | Target.LabelSelector      | &check;      |
| server         | Target.Server             | &check;      |
| targets        | List<Target.Target>       | &check;      |
| type           | String                    | &check;      |
| use_private_ip | Boolean                   | &check;      |

#### Target.HealthStatus
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| listen_port | Long     | &check;      |
| status      | String   | &check;      |

#### Target.Ip
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| ip       | String   | &check;      |

#### Target.LabelSelector
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| selector | String   | &check;      |

#### Target.Server
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |

#### Target.Target
| **Name**       | **Type**                         | **Nullable** |
| -------------- | -------------------------------- | ------------ |
| health_status  | List<Target.Target.HealthStatus> | &check;      |
| server         | Target.Target.Server             | &check;      |
| type           | String                           | &check;      |
| use_private_ip | Boolean                          | &check;      |

#### Target.Target.HealthStatus
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| listen_port | Long     | &check;      |
| status      | String   | &check;      |

#### Target.Target.Server
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |
