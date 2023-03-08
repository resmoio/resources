---
description: DigitalOcean Load Balancer
---
digitalocean_load_balancer
--------------------------

| **Name**                         | **Type**             | **Nullable** |
| -------------------------------- | -------------------- | ------------ |
| created_at                       | String               | &check;      |
| disable_lets_encrypt_dns_records | Boolean              | &check;      |
| droplet_ids                      | List<Int>            | &check;      |
| enable_backend_keepalive         | Boolean              | &check;      |
| enable_proxy_protocol            | Boolean              | &check;      |
| firewall                         | Firewall             | &check;      |
| forwarding_rules                 | List<ForwardingRule> | &check;      |
| health_check                     | HealthCheck          | &check;      |
| http_idle_timeout_seconds        | Int                  | &check;      |
| id                               | String               | &cross;      |
| ip                               | String               | &check;      |
| name                             | String               | &check;      |
| project_id                       | String               | &check;      |
| redirect_http_to_https           | Boolean              | &check;      |
| region                           | Region               | &check;      |
| size_unit                        | Int                  | &check;      |
| status                           | String               | &check;      |
| sticky_session                   | StickySession        | &check;      |
| tag                              | String               | &check;      |
| vpc_uuid                         | String               | &check;      |

#### Firewall
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| allow    | List<String> | &check;      |
| deny     | List<String> | &check;      |

#### ForwardingRule
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| certificate_id  | String   | &check;      |
| entry_port      | Long     | &check;      |
| entry_protocol  | String   | &check;      |
| target_port     | Int      | &check;      |
| target_protocol | String   | &check;      |
| tls_passthrough | Boolean  | &check;      |

#### HealthCheck
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| check_interval_seconds   | Long     | &check;      |
| healthy_threshold        | Int      | &check;      |
| path                     | String   | &check;      |
| port                     | Int      | &check;      |
| protocol                 | String   | &check;      |
| response_timeout_seconds | Long     | &check;      |
| unhealthy_threshold      | Int      | &check;      |

#### Region
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| available | Boolean      | &check;      |
| features  | List<String> | &check;      |
| name      | String       | &check;      |
| sizes     | List<String> | &check;      |
| slug      | String       | &check;      |

#### StickySession
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| cookie_name        | String   | &check;      |
| cookie_ttl_seconds | Long     | &check;      |
| type               | String   | &check;      |
