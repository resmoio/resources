---
description: Jotform Sub-User
---
jotform_sub_user
----------------

| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| created_at  | String           | &check;      |
| email       | String           | &cross;      |
| owner       | String           | &cross;      |
| permissions | List<Permission> | &check;      |
| status      | String           | &check;      |
| username    | String           | &cross;      |

#### Permission
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| resource_id | String   | &cross;      |
| title       | String   | &check;      |
| type        | String   | &cross;      |
