---
description: Cloudflare Zone Firewall Rule
---
cloudflare_zone_firewall_rule
-----------------------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| action      | String       | &check;      |
| description | String       | &check;      |
| filter      | Filter       | &check;      |
| id          | String       | &cross;      |
| paused      | Boolean      | &check;      |
| priority    | Int          | &check;      |
| products    | List<String> | &check;      |
| ref         | String       | &check;      |
| zone_id     | String       | &cross;      |

#### Filter
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| expression  | String   | &check;      |
| id          | String   | &check;      |
| paused      | Boolean  | &check;      |
| ref         | String   | &check;      |
