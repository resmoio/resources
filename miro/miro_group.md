---
description: Miro Group
---
miro_group
----------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| displayName  | String       | &check;      |
| id           | String       | &cross;      |
| members      | List<Member> | &check;      |
| meta         | Meta         | &check;      |
| name         | String       | &check;      |
| organization | String       | &check;      |
| schemas      | List<String> | &check;      |
| type         | String       | &check;      |

#### Member
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &cross;      |
| value    | String   | &cross;      |

#### Meta
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| location     | String   | &check;      |
| resourceType | String   | &check;      |
