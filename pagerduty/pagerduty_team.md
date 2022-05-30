---
description: PagerDuty Team
---
pagerduty_team
--------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| description | String       | &check;      |
| id          | String       | &cross;      |
| members     | List<Member> | &check;      |
| name        | String       | &check;      |
| parent      | Parent       | &check;      |
| summary     | String       | &check;      |
| type        | String       | &check;      |

#### Member
| **Name** | **Type**    | **Nullable** |
| -------- | ----------- | ------------ |
| role     | String      | &check;      |
| user     | Member.User | &check;      |

#### Member.User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| summary  | String   | &check;      |
| type     | String   | &check;      |

#### Parent
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| summary  | String   | &check;      |
| type     | String   | &check;      |
