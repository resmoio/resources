---
description: Segment User Group
---
segment_user_group
------------------

| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| id          | String           | &cross;      |
| memberCount | Int              | &check;      |
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
| **Name**  | **Type**                 | **Nullable** |
| --------- | ------------------------ | ------------ |
| resources | List<PermissionResource> | &check;      |
| roleId    | String                   | &cross;      |
| roleName  | String                   | &check;      |

#### PermissionResource
| **Name** | **Type**    | **Nullable** |
| -------- | ----------- | ------------ |
| id       | String      | &check;      |
| labels   | List<Label> | &check;      |
| type     | String      | &check;      |
