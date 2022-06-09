---
description: Cloudflare Zone User Agent Blocking Rule
---
cloudflare_zone_user_agent_blocking_rule
----------------------------------------

| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| configuration | Configuration | &check;      |
| description   | String        | &check;      |
| id            | String        | &cross;      |
| mode          | String        | &check;      |
| paused        | Boolean       | &check;      |
| zone_id       | String        | &cross;      |

#### Configuration
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| target   | String   | &check;      |
| value    | String   | &check;      |
