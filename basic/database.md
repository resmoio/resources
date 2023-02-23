---
description: Entity Database
---
database
--------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| encrypted          | Boolean            | &check;      |
| endpoint           | String             | &check;      |
| engine             | String             | &check;      |
| isPublic           | Boolean            | &check;      |
| name               | String             | &check;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |
| type               | String             | &cross;      |
| version            | String             | &check;      |

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

#### Type
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
| value    | String   | &cross;      |
