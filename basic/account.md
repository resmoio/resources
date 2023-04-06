---
description: Entity Account
---
account
-------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| accountType        | String             | &cross;      |
| createdAt          | String             | &check;      |
| id                 | String             | &cross;      |
| name               | String             | &check;      |
| plan               | String             | &check;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |

#### AccountType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |

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
