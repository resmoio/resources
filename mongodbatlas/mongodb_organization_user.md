---
description: MongoDB Atlas Organization User
---
mongodb_organization_user
-------------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| country      | String       | &check;      |
| emailAddress | String       | &check;      |
| firstName    | String       | &check;      |
| id           | String       | &cross;      |
| lastName     | String       | &check;      |
| links        | List<Link>   | &cross;      |
| mobileNumber | String       | &check;      |
| organization | Organization | &cross;      |
| roles        | List<Role>   | &cross;      |
| teamIds      | List<String> | &check;      |
| username     | String       | &check;      |

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
