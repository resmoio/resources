---
description: Entity User
---
user
----

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| active         | Boolean  | &check;      |
| data           | JSON     | &check;      |
| displayName    | String   | &check;      |
| email          | String   | &check;      |
| emailDomain    | String   | &check;      |
| firstName      | String   | &check;      |
| id             | String   | &cross;      |
| isAdmin        | Boolean  | &check;      |
| lastName       | String   | &check;      |
| lastSignIn     | String   | &check;      |
| mfaEnabled     | Boolean  | &check;      |
| referencedType | String   | &cross;      |
| type           | UserType | &check;      |
| userName       | String   | &check;      |

#### BasicResource
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| data           | JSON     | &check;      |
| referencedType | String   | &cross;      |

#### UserType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
