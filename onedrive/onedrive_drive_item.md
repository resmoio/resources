---
description: OneDrive Drive Item
---
onedrive_drive_item
-------------------

| **Name**             | **Type**         | **Nullable** |
| -------------------- | ---------------- | ------------ |
| createdBy            | IdentitySet      | &check;      |
| createdDateTime      | String           | &check;      |
| ctag                 | String           | &check;      |
| deleted              | Deleted          | &check;      |
| description          | String           | &check;      |
| driveId              | String           | &cross;      |
| etag                 | String           | &check;      |
| file                 | File             | &check;      |
| fileSystemInfo       | FileSystemInfo   | &check;      |
| folder               | Folder           | &check;      |
| id                   | String           | &cross;      |
| lastModifiedBy       | IdentitySet      | &check;      |
| lastModifiedDateTime | String           | &check;      |
| name                 | String           | &check;      |
| ownerUserId          | String           | &cross;      |
| package              | PackageInfo      | &check;      |
| parentReference      | ItemReference    | &check;      |
| permissions          | List<Permission> | &check;      |
| photo                | Photo            | &check;      |
| publication          | Publication      | &check;      |
| remoteItem           | JSON             | &check;      |
| sharePointIds        | SharePointIds    | &check;      |
| shared               | Shared           | &check;      |
| specialFolder        | SpecialFolder    | &check;      |
| type                 | String           | &cross;      |
| webDavUrl            | String           | &check;      |
| webUrl               | String           | &check;      |

#### Deleted
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| state    | String   | &check;      |

#### DriveItemType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |

#### File
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| mimeType           | String   | &check;      |
| processingMetadata | Boolean  | &check;      |

#### FileSystemInfo
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| createdDateTime      | String   | &check;      |
| lastAccessedDateTime | String   | &check;      |
| lastModifiedDateTime | String   | &check;      |

#### Folder
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| childCount | Int      | &check;      |

#### IdentitySet
| **Name**    | **Type**             | **Nullable** |
| ----------- | -------------------- | ------------ |
| application | IdentitySet.Identity | &check;      |
| device      | IdentitySet.Identity | &check;      |
| user        | IdentitySet.Identity | &check;      |

#### IdentitySet.Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |

#### ItemReference
| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| driveId       | String        | &check;      |
| driveType     | String        | &check;      |
| id            | String        | &check;      |
| name          | String        | &check;      |
| path          | String        | &check;      |
| shareId       | String        | &check;      |
| sharePointIds | SharePointIds | &check;      |
| siteId        | String        | &check;      |

#### PackageInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### Permission
| **Name**              | **Type**                               | **Nullable** |
| --------------------- | -------------------------------------- | ------------ |
| expirationDateTime    | String                                 | &check;      |
| grantedToIdentitiesV2 | List<Permission.SharePointIdentitySet> | &check;      |
| grantedToV2           | Permission.SharePointIdentitySet       | &check;      |
| hasPassword           | Boolean                                | &check;      |
| id                    | String                                 | &check;      |
| invitation            | Permission.Invitation                  | &check;      |
| link                  | Permission.SharingLink                 | &check;      |
| roles                 | List<String>                           | &check;      |
| shareId               | String                                 | &check;      |

#### Permission.Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |

#### Permission.Invitation
| **Name**       | **Type**    | **Nullable** |
| -------------- | ----------- | ------------ |
| email          | String      | &check;      |
| invitedBy      | IdentitySet | &check;      |
| signInRequired | Boolean     | &check;      |

#### Permission.SharePointIdentitySet
| **Name**    | **Type**                                            | **Nullable** |
| ----------- | --------------------------------------------------- | ------------ |
| application | Permission.Identity                                 | &check;      |
| device      | Permission.Identity                                 | &check;      |
| group       | Permission.Identity                                 | &check;      |
| siteGroup   | Permission.SharePointIdentitySet.SharePointIdentity | &check;      |
| siteUser    | Permission.SharePointIdentitySet.SharePointIdentity | &check;      |
| user        | Permission.Identity                                 | &check;      |

#### Permission.SharePointIdentitySet.SharePointIdentity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |
| loginName   | String   | &check;      |

#### Permission.SharingLink
| **Name**         | **Type**            | **Nullable** |
| ---------------- | ------------------- | ------------ |
| application      | Permission.Identity | &check;      |
| preventsDownload | Boolean             | &check;      |
| scope            | String              | &check;      |
| type             | String              | &check;      |

#### Photo
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| takenDateTime | String   | &check;      |

#### Publication
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| level     | String   | &check;      |
| versionId | String   | &check;      |

#### SharePointIds
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| listId           | String   | &check;      |
| listItemId       | String   | &check;      |
| listItemUniqueId | String   | &check;      |
| siteId           | String   | &check;      |
| siteUrl          | String   | &check;      |
| tenantId         | String   | &check;      |
| webId            | String   | &check;      |

#### Shared
| **Name**       | **Type**    | **Nullable** |
| -------------- | ----------- | ------------ |
| owner          | IdentitySet | &check;      |
| scope          | String      | &check;      |
| sharedBy       | IdentitySet | &check;      |
| sharedDateTime | String      | &check;      |

#### SpecialFolder
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
