---
description: Google Workspace Role
---
gsuite_role
-----------

| **Name**        | **Type**            | **Nullable** |
| --------------- | ------------------- | ------------ |
| customerId      | String              | &cross;      |
| isSystemRole    | Boolean             | &check;      |
| roleDescription | String              | &check;      |
| roleId          | String              | &cross;      |
| roleName        | String              | &cross;      |
| rolePrivileges  | List<RolePrivilege> | &check;      |

#### RolePrivilege
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| privilegeName | String   | &cross;      |
| serviceId     | String   | &cross;      |
