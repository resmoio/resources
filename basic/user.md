---
description: Entity User
---
user
----

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| active             | Boolean            | &check;      |
| displayName        | String             | &check;      |
| email              | String             | &check;      |
| emailDomain        | String             | &check;      |
| id                 | String             | &cross;      |
| isAdmin            | Boolean            | &check;      |
| lastSignIn         | String             | &check;      |
| mfaEnabled         | Boolean            | &check;      |
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
