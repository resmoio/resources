---
description: Cloudflare Zone Firewall Access Rule
---
cloudflare_zone_firewall_access_rule
------------------------------------

| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| allowed_modes | List<String>  | &check;      |
| configuration | Configuration | &check;      |
| created_on    | String        | &check;      |
| id            | String        | &cross;      |
| mode          | String        | &check;      |
| modified_on   | String        | &check;      |
| notes         | String        | &check;      |
| scope         | Scope         | &check;      |
| zone_id       | String        | &cross;      |

#### Configuration
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| target   | String   | &check;      |
| value    | String   | &check;      |

#### Scope
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |
| type     | String   | &check;      |
