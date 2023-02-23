---
description: Zoom Role
---
zoom_role
---------

| **Name**             | **Type**             | **Nullable** |
| -------------------- | -------------------- | ------------ |
| description          | String               | &check;      |
| id                   | String               | &cross;      |
| name                 | String               | &check;      |
| privileges           | List<String>         | &check;      |
| subAccountPrivileges | SubAccountPrivileges | &check;      |
| totalMembers         | Int                  | &check;      |

#### SubAccountPrivileges
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| secondLevel | Int      | &check;      |
