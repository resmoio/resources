---
description: Opsgenie Team
---
opsgenie_team
-------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| accountName | String       | &check;      |
| description | String       | &cross;      |
| id          | String       | &cross;      |
| members     | List<Member> | &check;      |
| name        | String       | &cross;      |
| roles       | List<Role>   | &check;      |

#### Member
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| role     | String   | &check;      |
| user     | User     | &check;      |

#### Role
| **Name** | **Type**            | **Nullable** |
| -------- | ------------------- | ------------ |
| id       | String              | &check;      |
| name     | String              | &check;      |
| rights   | Map<String,Boolean> | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| username | String   | &check;      |
