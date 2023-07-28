---
description: OneDrive Drive
---
onedrive_drive
--------------

| **Name**             | **Type**      | **Nullable** |
| -------------------- | ------------- | ------------ |
| createdBy            | IdentitySet   | &check;      |
| createdDateTime      | String        | &check;      |
| description          | String        | &check;      |
| driveType            | String        | &check;      |
| id                   | String        | &cross;      |
| lastModifiedBy       | IdentitySet   | &check;      |
| lastModifiedDateTime | String        | &check;      |
| name                 | String        | &check;      |
| oDataType            | String        | &check;      |
| owner                | IdentitySet   | &check;      |
| quota                | Quota         | &check;      |
| sharepointIds        | SharePointIds | &check;      |
| webUrl               | String        | &check;      |

#### IdentitySet
| **Name**    | **Type**             | **Nullable** |
| ----------- | -------------------- | ------------ |
| application | IdentitySet.Identity | &check;      |
| device      | IdentitySet.Identity | &check;      |
| oDataType   | String               | &check;      |
| user        | IdentitySet.Identity | &check;      |

#### IdentitySet.Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |

#### Quota
| **Name**               | **Type**                     | **Nullable** |
| ---------------------- | ---------------------------- | ------------ |
| oDataType              | String                       | &check;      |
| state                  | String                       | &check;      |
| storagePlanInformation | Quota.StoragePlanInformation | &check;      |
| total                  | Long                         | &check;      |

#### Quota.StoragePlanInformation
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| oDataType        | String   | &check;      |
| upgradeAvailable | Boolean  | &check;      |

#### SharePointIds
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| listId           | String   | &check;      |
| listItemId       | String   | &check;      |
| listItemUniqueId | String   | &check;      |
| oDataType        | String   | &check;      |
| siteId           | String   | &check;      |
| siteUrl          | String   | &check;      |
| tenantId         | String   | &check;      |
| webId            | String   | &check;      |
