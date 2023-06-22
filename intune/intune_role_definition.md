---
description: Intune Role Definition
---
intune_role_definition
----------------------

| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| description     | String               | &check;      |
| displayName     | String               | &check;      |
| id              | String               | &cross;      |
| isBuiltIn       | Boolean              | &check;      |
| rolePermissions | List<RolePermission> | &check;      |

#### ResourceAction
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| allowedResourceActions    | List<String> | &check;      |
| notAllowedResourceActions | List<String> | &check;      |

#### RolePermission
| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| resourceActions | List<ResourceAction> | &check;      |
