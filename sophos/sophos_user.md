---
description: Sophos User
---
sophos_user
-----------

| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| createdAt       | String               | &check;      |
| domain          | String               | &check;      |
| email           | String               | &check;      |
| exchangeLogin   | String               | &check;      |
| firstName       | String               | &check;      |
| groups          | Groups               | &check;      |
| id              | String               | &cross;      |
| isAdmin         | Boolean              | &check;      |
| lastName        | String               | &check;      |
| name            | String               | &check;      |
| roleAssignments | List<RoleAssignment> | &check;      |
| source          | Source               | &check;      |
| tenant          | Tenant               | &cross;      |
| updatedAt       | String               | &check;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |

#### Groups
| **Name**   | **Type**    | **Nullable** |
| ---------- | ----------- | ------------ |
| items      | List<Group> | &check;      |
| itemsCount | Int         | &check;      |
| total      | Int         | &check;      |

#### RoleAssignment
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| roleId   | String   | &cross;      |

#### Source
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### Tenant
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
