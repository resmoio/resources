---
description: MongoDB Atlas Organization Team
---
mongodb_team
------------

| **Name**     | **Type**       | **Nullable** |
| ------------ | -------------- | ------------ |
| id           | String         | &cross;      |
| links        | List<Link>     | &cross;      |
| name         | String         | &check;      |
| organization | Organization   | &cross;      |
| users        | List<TeamUser> | &cross;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupId  | String   | &check;      |
| orgId    | String   | &check;      |
| roleName | String   | &check;      |

#### TeamUser
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| country      | String       | &check;      |
| emailAddress | String       | &check;      |
| firstName    | String       | &check;      |
| id           | String       | &check;      |
| lastName     | String       | &check;      |
| links        | List<Link>   | &cross;      |
| roles        | List<Role>   | &cross;      |
| teamIds      | List<String> | &cross;      |
| username     | String       | &check;      |
