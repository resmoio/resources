---
description: MonoSign User Role
---
monosign_user_role
------------------

| **Name**     | **Type**       | **Nullable** |
| ------------ | -------------- | ------------ |
| description  | String         | &check;      |
| endDate      | String         | &check;      |
| name         | String         | &check;      |
| objectId     | String         | &check;      |
| objectTypeId | String         | &check;      |
| roleDef      | RoleDefinition | &check;      |
| roleDefId    | String         | &check;      |
| roleId       | String         | &cross;      |
| startDate    | String         | &check;      |
| title        | String         | &check;      |
| userId       | String         | &check;      |

#### RoleDefinition
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| name        | String   | &check;      |
| roleDefId   | String   | &check;      |
| state       | Int      | &check;      |
| title       | String   | &check;      |
