---
description: MongoDB Atlas Project
---
mongodb_project
---------------

| **Name**     | **Type**          | **Nullable** |
| ------------ | ----------------- | ------------ |
| clusterCount | Int               | &check;      |
| created      | String            | &check;      |
| id           | String            | &cross;      |
| links        | List<Link>        | &cross;      |
| name         | String            | &check;      |
| orgId        | String            | &check;      |
| settings     | ProjectSettings   | &cross;      |
| users        | List<ProjectUser> | &cross;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### ProjectInvitation
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| createdAt       | String       | &check;      |
| expiresAt       | String       | &check;      |
| groupId         | String       | &check;      |
| groupName       | String       | &check;      |
| id              | String       | &check;      |
| inviterUsername | String       | &check;      |
| roles           | List<String> | &cross;      |
| username        | String       | &check;      |

#### ProjectSettings
| **Name**                                    | **Type** | **Nullable** |
| ------------------------------------------- | -------- | ------------ |
| isCollectDatabaseSpecificsStatisticsEnabled | Boolean  | &check;      |
| isDataExplorerEnabled                       | Boolean  | &check;      |
| isPerformanceAdvisorEnabled                 | Boolean  | &check;      |
| isRealtimePerformancePanelEnabled           | Boolean  | &check;      |
| isSchemaAdvisorEnabled                      | Boolean  | &check;      |

#### ProjectUser
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| country      | String       | &check;      |
| emailAddress | String       | &check;      |
| firstName    | String       | &check;      |
| id           | String       | &check;      |
| lastName     | String       | &check;      |
| links        | List<Link>   | &cross;      |
| orgId        | String       | &check;      |
| roles        | List<Role>   | &cross;      |
| teamIds      | List<String> | &cross;      |
| username     | String       | &check;      |

#### Role
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupId  | String   | &check;      |
| orgId    | String   | &check;      |
| roleName | String   | &check;      |
