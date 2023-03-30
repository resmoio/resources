---
description: Sophos User Group
---
sophos_user_group
-----------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| createdAt     | String   | &check;      |
| description   | String   | &check;      |
| domain        | String   | &check;      |
| exchangeLogin | String   | &check;      |
| id            | String   | &cross;      |
| name          | String   | &check;      |
| tenant        | Tenant   | &cross;      |
| updatedAt     | String   | &check;      |
| users         | Users    | &check;      |

#### Tenant
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |

#### Users
| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| items      | List<User> | &check;      |
| itemsCount | Int        | &check;      |
| total      | Int        | &check;      |
