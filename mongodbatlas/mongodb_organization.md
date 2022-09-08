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
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| emailAddress | String   | &check;      |
| id           | String   | &check;      |
| username     | String   | &check;      |

#### Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupId  | String   | &check;      |
| orgId    | String   | &check;      |
| roleName | String   | &check;      |
