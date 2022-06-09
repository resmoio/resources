---
description: Cloudflare Zone Transform Rule
---
cloudflare_zone_transform_rule
------------------------------

| **Name**     | **Type**   | **Nullable** |
| ------------ | ---------- | ------------ |
| description  | String     | &check;      |
| id           | String     | &cross;      |
| kind         | String     | &check;      |
| last_updated | String     | &check;      |
| phase        | String     | &check;      |
| rules        | List<Rule> | &check;      |
| version      | String     | &check;      |
| zone_id      | String     | &cross;      |

#### Rule
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| action            | String   | &check;      |
| action_parameters | JSON     | &check;      |
| description       | String   | &check;      |
| expression        | String   | &check;      |
| id                | String   | &check;      |
| version           | String   | &check;      |
