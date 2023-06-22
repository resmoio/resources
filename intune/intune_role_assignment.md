---
description: Intune Role Assignment
---
intune_role_assignment
----------------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| description    | String         | &check;      |
| displayName    | String         | &check;      |
| id             | String         | &cross;      |
| members        | List<String>   | &check;      |
| resourceScopes | List<String>   | &check;      |
| roleDefinition | RoleDefinition | &check;      |

#### RoleDefinition
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| displayName | String   | &check;      |
| id          | String   | &cross;      |
| isBuiltIn   | Boolean  | &check;      |
