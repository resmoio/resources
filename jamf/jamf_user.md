---
description: Jamf Pro User
---
jamf_user
---------

| **Name**             | **Type**                 | **Nullable** |
| -------------------- | ------------------------ | ------------ |
| customPhotoUrl       | String                   | &check;      |
| email                | String                   | &check;      |
| emailAddress         | String                   | &check;      |
| enableCustomPhotoUrl | Boolean                  | &check;      |
| extensionAttributes  | List<ExtensionAttribute> | &check;      |
| fullName             | String                   | &check;      |
| id                   | Int                      | &cross;      |
| ldapServer           | LdapServer               | &check;      |
| links                | Links                    | &check;      |
| managedAppleId       | String                   | &check;      |
| name                 | String                   | &check;      |
| phoneNumber          | String                   | &check;      |
| position             | String                   | &check;      |
| serverName           | String                   | &cross;      |
| sites                | List<Site>               | &check;      |
| userGroups           | UserGroups               | &check;      |

#### ExtensionAttribute
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
| value    | String   | &check;      |

#### LdapServer
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Links
| **Name**          | **Type**   | **Nullable** |
| ----------------- | ---------- | ------------ |
| computers         | List<Site> | &check;      |
| mobileDevices     | List<Site> | &check;      |
| peripherals       | List<Site> | &check;      |
| totalVppCodeCount | Int        | &check;      |
| vppAssignments    | List<Site> | &check;      |

#### Site
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### UserGroups
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| size     | Int      | &check;      |
