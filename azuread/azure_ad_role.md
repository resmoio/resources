---
description: Azure Active Directory Role
---
azure_ad_role
-------------

| **Name**       | **Type**                   | **Nullable** |
| -------------- | -------------------------- | ------------ |
| description    | String                     | &check;      |
| displayName    | String                     | &check;      |
| id             | String                     | &cross;      |
| members        | List<DirectoryObject>      | &check;      |
| oDataType      | String                     | &check;      |
| roleTemplateId | String                     | &check;      |
| scopedMembers  | List<ScopedRoleMembership> | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |

#### Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |

#### ScopedRoleMembership
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| administrativeUnitId | String   | &check;      |
| id                   | String   | &check;      |
| oDataType            | String   | &check;      |
| roleId               | String   | &check;      |
| roleMemberInfo       | Identity | &check;      |
