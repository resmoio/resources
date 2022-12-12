---
description: Kandji Device
---
kandji_device
-------------

| **Name**          | **Type**               | **Nullable** |
| ----------------- | ---------------------- | ------------ |
| activationLock    | Map<String,Boolean>    | &check;      |
| agentInstalled    | Boolean                | &check;      |
| agentVersion      | String                 | &check;      |
| assetTag          | String                 | &check;      |
| blueprintId       | String                 | &check;      |
| blueprintName     | String                 | &check;      |
| fileVault         | FileVault              | &check;      |
| firstEnrollment   | String                 | &check;      |
| hardwareOverview  | Map<String,String>     | &check;      |
| id                | String                 | &cross;      |
| installedProfiles | List<InstalledProfile> | &check;      |
| isMissing         | Boolean                | &check;      |
| isRemoved         | Boolean                | &check;      |
| kandjiAgent       | Map<String,String>     | &check;      |
| lastCheckIn       | String                 | &check;      |
| lastEnrollment    | String                 | &check;      |
| mdm               | Mdm                    | &check;      |
| model             | String                 | &check;      |
| name              | String                 | &check;      |
| network           | Map<String,String>     | &check;      |
| osVersion         | String                 | &check;      |
| parameters        | List<Parameter>        | &check;      |
| platform          | String                 | &check;      |
| serialNumber      | String                 | &check;      |
| user              | User                   | &check;      |
| users             | Users                  | &check;      |
| volumes           | List<Map>              | &check;      |

#### FileVault
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| fileVaultEnabled         | Boolean  | &check;      |
| filevaultNextRotation    | String   | &check;      |
| filevaultPrkEscrowed     | Boolean  | &check;      |
| filevaultRecoverykeyType | String   | &check;      |
| filevaultRegenRequired   | Boolean  | &check;      |

#### InstalledProfile
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| identifier   | String       | &check;      |
| installDate  | String       | &check;      |
| name         | String       | &check;      |
| organization | String       | &check;      |
| payloadTypes | List<String> | &check;      |
| uuid         | String       | &cross;      |
| verified     | String       | &check;      |

#### Mdm
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| installDate    | String       | &check;      |
| lastCheckIn    | String       | &check;      |
| mdmEnabled     | String       | &check;      |
| mdmEnabledUser | List<String> | &check;      |

#### Parameter
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| category    | String   | &check;      |
| itemId      | String   | &check;      |
| name        | String   | &check;      |
| status      | String   | &check;      |
| subcategory | String   | &check;      |

#### RegularUser
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| admin    | String   | &check;      |
| name     | String   | &check;      |
| path     | String   | &check;      |
| uid      | String   | &cross;      |
| username | String   | &cross;      |

#### SystemUser
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| admin    | String   | &check;      |
| path     | String   | &check;      |
| uid      | String   | &cross;      |
| username | String   | &check;      |

#### User
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| deviceId   | String   | &check;      |
| email      | String   | &check;      |
| id         | Long     | &cross;      |
| isArchived | Boolean  | &check;      |
| username   | String   | &check;      |

#### Users
| **Name**     | **Type**          | **Nullable** |
| ------------ | ----------------- | ------------ |
| regularUsers | List<RegularUser> | &check;      |
| systemUsers  | List<SystemUser>  | &check;      |
