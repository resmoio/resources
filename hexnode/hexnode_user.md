---
description: Hexnode User
---
hexnode_user
------------

| **Name**         | **Type**              | **Nullable** |
| ---------------- | --------------------- | ------------ |
| devices          | List<Device>          | &check;      |
| domain           | String                | &check;      |
| email            | String                | &check;      |
| groups           | List<Group>           | &check;      |
| id               | String                | &cross;      |
| location_history | List<LocationHistory> | &check;      |
| name             | String                | &check;      |
| phoneno          | String                | &check;      |
| policies         | List<Policy>          | &check;      |
| upn              | String                | &check;      |

#### Device
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| id         | Int      | &cross;      |
| model_name | String   | &check;      |
| name       | String   | &check;      |
| platform   | String   | &check;      |
| status     | String   | &check;      |

#### Group
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| created_date | String   | &check;      |
| description  | String   | &check;      |
| id           | Int      | &cross;      |
| name         | String   | &check;      |

#### LocationHistory
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| device_id          | Int      | &check;      |
| device_name        | String   | &check;      |
| last_location      | String   | &check;      |
| last_location_time | String   | &check;      |
| latitude           | String   | &check;      |
| longitude          | String   | &check;      |

#### Policy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &cross;      |
| name     | String   | &check;      |
| version  | Int      | &check;      |
