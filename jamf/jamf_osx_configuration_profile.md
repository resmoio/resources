---
description: Jamf Pro OSX Configuration Profile
---
jamf_osx_configuration_profile
------------------------------

| **Name**           | **Type**    | **Nullable** |
| ------------------ | ----------- | ------------ |
| category           | Category    | &check;      |
| description        | String      | &check;      |
| distributionMethod | String      | &check;      |
| id                 | Int         | &cross;      |
| level              | String      | &check;      |
| name               | String      | &check;      |
| payloads           | String      | &check;      |
| redeployOnUpdate   | String      | &check;      |
| scope              | Scope       | &check;      |
| selfService        | SelfService | &check;      |
| serverName         | String      | &cross;      |
| site               | Site        | &check;      |
| userRemovable      | Boolean     | &check;      |
| uuid               | String      | &check;      |

#### Building
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Category
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Computer
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| udid     | String   | &check;      |

#### ComputerGroup
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Department
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Exclusions
| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| buildings       | List<Building>       | &check;      |
| computerGroups  | List<ComputerGroup>  | &check;      |
| computers       | List<Computer>       | &check;      |
| departments     | List<Department>     | &check;      |
| ibeacons        | List<Ibeacon>        | &check;      |
| jssUserGroups   | List<UserGroup>      | &check;      |
| jssUsers        | List<User>           | &check;      |
| networkSegments | List<NetworkSegment> | &check;      |
| userGroups      | List<UserGroup>      | &check;      |
| users           | List<User>           | &check;      |

#### Ibeacon
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Limitations
| **Name**        | **Type**             | **Nullable** |
| --------------- | -------------------- | ------------ |
| ibeacons        | List<Ibeacon>        | &check;      |
| networkSegments | List<NetworkSegment> | &check;      |
| userGroups      | List<UserGroup>      | &check;      |
| users           | List<User>           | &check;      |

#### NetworkSegment
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| uid      | String   | &check;      |

#### Scope
| **Name**       | **Type**            | **Nullable** |
| -------------- | ------------------- | ------------ |
| allComputers   | Boolean             | &check;      |
| allJssUsers    | Boolean             | &check;      |
| buildings      | List<Building>      | &check;      |
| computerGroups | List<ComputerGroup> | &check;      |
| computers      | List<Computer>      | &check;      |
| departments    | List<Department>    | &check;      |
| exclusions     | Exclusions          | &check;      |
| jssUserGroups  | List<UserGroup>     | &check;      |
| jssUsers       | List<User>          | &check;      |
| limitations    | Limitations         | &check;      |

#### SelfService
| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| featureOnMainPage           | Boolean                     | &check;      |
| forceUsersToViewDescription | Boolean                     | &check;      |
| installButtonText           | String                      | &check;      |
| notification                | String                      | &check;      |
| notificationMessage         | String                      | &check;      |
| notificationSubject         | String                      | &check;      |
| selfServiceCategories       | List<SelfServiceCategories> | &check;      |
| selfServiceDescription      | String                      | &check;      |
| selfServiceIcon             | SelfServiceIcon             | &check;      |

#### SelfServiceCategories
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| displayIn | Boolean  | &check;      |
| featureIn | Boolean  | &check;      |
| id        | Int      | &check;      |
| name      | String   | &check;      |

#### SelfServiceIcon
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| data     | String   | &check;      |
| id       | Int      | &check;      |
| uri      | String   | &check;      |

#### Site
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### UserGroup
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
