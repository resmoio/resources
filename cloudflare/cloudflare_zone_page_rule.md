---
description: Cloudflare Zone Page Rule
---
cloudflare_zone_page_rule
-------------------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| actions     | List<Action> | &check;      |
| created_On  | String       | &check;      |
| id          | String       | &cross;      |
| modified_on | String       | &check;      |
| priority    | Int          | &check;      |
| status      | String       | &check;      |
| targets     | List<Target> | &check;      |
| zone_id     | String       | &cross;      |

#### Action
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| value    | JSON     | &check;      |

#### Target
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| constraints | JSON     | &check;      |
| target      | String   | &check;      |
