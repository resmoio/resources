---
description: Asana User
---
asana_user
----------

| **Name**      | **Type**        | **Nullable** |
| ------------- | --------------- | ------------ |
| email         | String          | &check;      |
| gid           | String          | &cross;      |
| name          | String          | &cross;      |
| resource_type | String          | &cross;      |
| teams         | List<Team>      | &check;      |
| workspaces    | List<Workspace> | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gid      | String   | &cross;      |
| name     | String   | &cross;      |

#### Workspace
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gid      | String   | &cross;      |
| name     | String   | &cross;      |
