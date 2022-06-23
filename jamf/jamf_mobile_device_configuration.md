---
description: Jamf Pro Mobile Device Configuration
---
jamf_mobile_device_configuration
--------------------------------

| **Name**                             | **Type**    | **Nullable** |
| ------------------------------------ | ----------- | ------------ |
| category                             | Category    | &check;      |
| deploymentMethod                     | String      | &check;      |
| description                          | String      | &check;      |
| id                                   | Int         | &cross;      |
| level                                | String      | &check;      |
| name                                 | String      | &check;      |
| payloads                             | String      | &check;      |
| redeployDaysBeforeCertificateExpires | Int         | &check;      |
| redeployOnUpdate                     | String      | &check;      |
| scope                                | Scope       | &check;      |
| selfService                          | SelfService | &check;      |
| serverName                           | String      | &cross;      |
| site                                 | Site        | &check;      |
| uuid                                 | String      | &check;      |

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

#### Department
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Exclusions
| **Name**           | **Type**                | **Nullable** |
| ------------------ | ----------------------- | ------------ |
| buildings          | List<Building>          | &check;      |
| departments        | List<Department>        | &check;      |
| ibeacons           | List<Ibeacon>           | &check;      |
| jssUserGroups      | List<UserGroup>         | &check;      |
| jssUsers           | List<User>              | &check;      |
| mobileDeviceGroups | List<MobileDeviceGroup> | &check;      |
| mobileDevices      | List<MobileDevice>      | &check;      |
| networkSegments    | List<NetworkSegment>    | &check;      |
| userGroups         | List<UserGroup>         | &check;      |
| users              | List<User>              | &check;      |

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

#### MobileDevice
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| id             | Int      | &check;      |
| name           | String   | &check;      |
| udid           | String   | &check;      |
| wifiMacAddress | String   | &check;      |

#### MobileDeviceGroup
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### NetworkSegment
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| uid      | String   | &check;      |

#### Scope
| **Name**           | **Type**                | **Nullable** |
| ------------------ | ----------------------- | ------------ |
| allJssUsers        | Boolean                 | &check;      |
| allMobileDevices   | Boolean                 | &check;      |
| buildings          | List<Building>          | &check;      |
| departments        | List<Department>        | &check;      |
| exclusions         | Exclusions              | &check;      |
| jssUserGroups      | List<UserGroup>         | &check;      |
| jssUsers           | List<User>              | &check;      |
| limitations        | Limitations             | &check;      |
| mobileDeviceGroups | List<MobileDeviceGroup> | &check;      |
| mobileDevices      | List<MobileDevice>      | &check;      |

#### SecurityName
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| removalDisallowed | String   | &check;      |

#### SelfService
| **Name**               | **Type**                  | **Nullable** |
| ---------------------- | ------------------------- | ------------ |
| featureOnMainPage      | Boolean                   | &check;      |
| securityName           | SecurityName              | &check;      |
| selfServiceCategories  | List<SelfServiceCategory> | &check;      |
| selfServiceDescription | String                    | &check;      |
| selfServiceIcon        | SelfServiceIcon           | &check;      |

#### SelfServiceCategory
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| priority | Int      | &check;      |

#### SelfServiceIcon
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| data     | String   | &check;      |
| filename | String   | &check;      |
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
