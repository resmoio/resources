---
description: MongoDB Atlas Organization
---
mongodb_organization
--------------------

| **Name**  | **Type**                  | **Nullable** |
| --------- | ------------------------- | ------------ |
| id        | String                    | &cross;      |
| isDeleted | Boolean                   | &check;      |
| links     | List<Link>                | &cross;      |
| name      | String                    | &check;      |
| projects  | List<OrganizationProject> | &cross;      |
| users     | List<OrganizationUser>    | &cross;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### OrganizationProject
| **Name**     | **Type**   | **Nullable** |
| ------------ | ---------- | ------------ |
| clusterCount | Int        | &check;      |
| created      | String     | &check;      |
| id           | String     | &check;      |
| links        | List<Link> | &cross;      |
| name         | String     | &check;      |
| orgId        | String     | &check;      |

#### OrganizationUser
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| country      | String       | &check;      |
| emailAddress | String       | &check;      |
| firstName    | String       | &check;      |
| id           | String       | &check;      |
| lastName     | String       | &check;      |
| links        | List<Link>   | &cross;      |
| mobileNumber | String       | &check;      |
| roles        | List<Role>   | &cross;      |
| teamIds      | List<String> | &check;      |
| username     | String       | &check;      |

#### Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupId  | String   | &check;      |
| orgId    | String   | &check;      |
| roleName | String   | &check;      |
