---
description: Hexnode Device Group
---
hexnode_device_group
--------------------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| description | String       | &check;      |
| devices     | List<Device> | &check;      |
| groupname   | String       | &check;      |
| id          | String       | &cross;      |
| policy      | List<Policy> | &check;      |

#### Device
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| id         | Int      | &check;      |
| model_name | String   | &check;      |
| name       | String   | &check;      |
| platform   | String   | &check;      |
| user_id    | String   | &check;      |
| user_name  | String   | &check;      |

#### Policy
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| cerated_time | String   | &check;      |
| id           | Int      | &cross;      |
| name         | String   | &check;      |
| version      | Int      | &check;      |
