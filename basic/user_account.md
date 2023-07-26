---
description: Entity User Account
---
user_account
------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| active             | Boolean            | &check;      |
| alternativeEmails  | List<String>       | &check;      |
| displayName        | String             | &check;      |
| email              | String             | &check;      |
| emailDomain        | String             | &check;      |
| id                 | String             | &cross;      |
| isAdmin            | Boolean            | &check;      |
| isDeleted          | Boolean            | &cross;      |
| isDirectoryUser    | Boolean            | &cross;      |
| lastSignIn         | String             | &check;      |
| mfaEnabled         | Boolean            | &check;      |
| phoneNumber        | String             | &check;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |
| type               | String             | &check;      |
| userName           | String             | &check;      |

#### BasicResource
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |

#### ReferencedResource
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| groupKey      | String   | &cross;      |
| integrationId | String   | &cross;      |
| recordId      | String   | &cross;      |
| resourceId    | String   | &cross;      |
| resourceType  | String   | &cross;      |

#### UserType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
