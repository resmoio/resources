---
description: Entity Repository
---
repository
----------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| id                 | String             | &cross;      |
| license            | String             | &check;      |
| name               | String             | &check;      |
| organization       | String             | &check;      |
| public             | Boolean            | &check;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |

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
