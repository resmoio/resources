---
description: DigitalOcean Firewall
---
digitalocean_firewall
---------------------

| **Name**        | **Type**        | **Nullable** |
| --------------- | --------------- | ------------ |
| created_at      | String          | &check;      |
| droplet_ids     | List<Int>       | &check;      |
| id              | String          | &cross;      |
| inbound_rules   | List<Inbounds>  | &check;      |
| name            | String          | &check;      |
| outbound_rules  | List<Outbounds> | &check;      |
| pending_changes | List<Changes>   | &check;      |
| status          | String          | &check;      |
| tags            | List<String>    | &check;      |

#### Changes
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| droplet_id | String   | &check;      |
| removing   | Boolean  | &check;      |
| status     | String   | &check;      |

#### Inbounds
| **Name** | **Type**            | **Nullable** |
| -------- | ------------------- | ------------ |
| ports    | String              | &check;      |
| protocol | String              | &check;      |
| sources  | SourceOrDestination | &check;      |

#### Outbounds
| **Name**     | **Type**            | **Nullable** |
| ------------ | ------------------- | ------------ |
| destinations | SourceOrDestination | &check;      |
| ports        | String              | &check;      |
| protocol     | String              | &check;      |

#### SourceOrDestination
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| addresses         | List<String> | &check;      |
| droplet_ids       | List<Int>    | &check;      |
| kubernetes_ids    | List<String> | &check;      |
| load_balancer_ids | List<String> | &check;      |
| tags              | List<String> | &check;      |
