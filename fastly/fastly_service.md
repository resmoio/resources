---
description: Fastly Service
---
fastly_service
--------------

| **Name**    | **Type**      | **Nullable** |
| ----------- | ------------- | ------------ |
| comment     | String        | &check;      |
| created_at  | String        | &check;      |
| customer_id | String        | &check;      |
| id          | String        | &cross;      |
| name        | String        | &check;      |
| paused      | Boolean       | &check;      |
| type        | String        | &check;      |
| updated_at  | String        | &check;      |
| version     | Int           | &check;      |
| versions    | List<Version> | &check;      |

#### Version
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| active     | Boolean  | &check;      |
| comment    | String   | &check;      |
| created_at | String   | &check;      |
| deleted_at | String   | &check;      |
| deployed   | Boolean  | &check;      |
| locked     | Boolean  | &check;      |
| number     | Int      | &check;      |
| service_id | String   | &check;      |
| staging    | Boolean  | &check;      |
| testing    | Boolean  | &check;      |
| updated_at | String   | &check;      |
