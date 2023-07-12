---
description: Google Workspace Privilege
---
gsuite_privilege
----------------

| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| childPrivileges | List<ChildPrivilege> | &check;      |
| customerId      | String               | &cross;      |
| isOuScopable    | Boolean              | &cross;      |
| privilegeName   | String               | &cross;      |
| serviceId       | String               | &check;      |
| serviceName     | String               | &check;      |

#### ChildPrivilege
| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| childPrivileges | List<ChildPrivilege> | &check;      |
| isOuScopable    | Boolean              | &check;      |
| privilegeName   | String               | &check;      |
| serviceId       | String               | &check;      |
| serviceName     | String               | &check;      |
