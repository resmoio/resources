---
description: CrowdStrike User
---
crowdstrike_user
----------------

| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| cid        | String     | &check;      |
| created_at | String     | &check;      |
| first_name | String     | &check;      |
| last_name  | String     | &check;      |
| roles      | List<Role> | &check;      |
| uid        | String     | &cross;      |
| uuid       | String     | &cross;      |

#### Role
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| grant_type | String   | &cross;      |
| role_id    | String   | &cross;      |
