---
description: DigitalOcean Project
---
digitalocean_project
--------------------

| **Name**    | **Type**              | **Nullable** |
| ----------- | --------------------- | ------------ |
| created_at  | String                | &check;      |
| description | String                | &check;      |
| environment | String                | &check;      |
| id          | String                | &cross;      |
| is_default  | String                | &check;      |
| name        | String                | &check;      |
| owner_id    | String                | &check;      |
| owner_uuid  | String                | &check;      |
| purpose     | String                | &check;      |
| resources   | List<ProjectResource> | &check;      |
| updated_at  | String                | &check;      |

#### ProjectResource
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| assigned_at | String   | &check;      |
| status      | String   | &check;      |
| urn         | String   | &check;      |
