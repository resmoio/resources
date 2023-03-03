---
description: Bitbucket Group
---
bitbucket_group
---------------

| **Name**                  | **Type**        | **Nullable** |
| ------------------------- | --------------- | ------------ |
| auto_add                  | Boolean         | &check;      |
| email_forwarding_disabled | Boolean         | &check;      |
| members                   | List<Member>    | &cross;      |
| name                      | String          | &check;      |
| owner                     | Owner           | &cross;      |
| permission                | String          | &check;      |
| privileges                | List<Privilege> | &check;      |
| slug                      | String          | &cross;      |
| workspace_id              | String          | &cross;      |
| workspace_name            | String          | &check;      |

#### Member
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_id   | String   | &check;      |
| display_name | String   | &check;      |
| nickname     | String   | &check;      |
| uuid         | String   | &cross;      |

#### Owner
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| display_name | String   | &check;      |
| is_team      | Boolean  | &check;      |
| nickname     | String   | &check;      |
| uuid         | String   | &cross;      |

#### Privilege
| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| privilege  | String     | &cross;      |
| repo       | String     | &cross;      |
| repository | Repository | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| owner    | Owner    | &check;      |
| slug     | String   | &check;      |
