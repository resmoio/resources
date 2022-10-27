---
description: Tenable.io Permission
---
tenable_permission
------------------

| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| actions         | List<String> | &check;      |
| created_at      | String       | &check;      |
| created_by      | String       | &check;      |
| name            | String       | &check;      |
| objects         | List<Info>   | &check;      |
| permission_uuid | String       | &cross;      |
| subjects        | List<Info>   | &check;      |
| updated_at      | String       | &check;      |
| updated_by      | String       | &check;      |

#### Info
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |
| uuid     | String   | &check;      |
