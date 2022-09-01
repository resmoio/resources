---
description: Entity Database
---
database
--------

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| data           | JSON     | &check;      |
| encrypted      | Boolean  | &check;      |
| endpoint       | String   | &check;      |
| engine         | String   | &check;      |
| isPublic       | Boolean  | &check;      |
| name           | String   | &check;      |
| referencedType | String   | &cross;      |
| type           | Type     | &cross;      |
| version        | String   | &check;      |

#### BasicResource
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| data           | JSON     | &check;      |
| referencedType | String   | &cross;      |

#### Type
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
| value    | String   | &cross;      |
