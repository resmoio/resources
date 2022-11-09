---
description: Segment User
---
segment_user
------------

| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| email       | String           | &check;      |
| groups      | List<String>     | &check;      |
| id          | String           | &cross;      |
| name        | String           | &check;      |
| permissions | List<Permission> | &check;      |
| workspaceId | String           | &check;      |

#### Label
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| key         | String   | &check;      |
| value       | String   | &check;      |

#### Permission
| **Name**  | **Type**       | **Nullable** |
| --------- | -------------- | ------------ |
| resources | List<Resource> | &check;      |
| roleId    | String         | &cross;      |
| roleName  | String         | &check;      |

#### Resource
| **Name** | **Type**    | **Nullable** |
| -------- | ----------- | ------------ |
| id       | String      | &check;      |
| labels   | List<Label> | &check;      |
| type     | String      | &check;      |
