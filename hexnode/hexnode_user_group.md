---
description: Hexnode User Group
---
hexnode_user_group
------------------

| **Name**      | **Type**   | **Nullable** |
| ------------- | ---------- | ------------ |
| description   | String     | &check;      |
| groupname     | String     | &check;      |
| id            | String     | &cross;      |
| modified_date | String     | &check;      |
| users         | List<User> | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &check;      |
| email    | String   | &check;      |
| id       | Int      | &cross;      |
| name     | String   | &check;      |
| phoneno  | String   | &check;      |
