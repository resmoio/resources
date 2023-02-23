---
description: Entity Container
---
container
---------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| args               | List<String>       | &check;      |
| command            | List<String>       | &check;      |
| cpus               | String             | &check;      |
| id                 | String             | &cross;      |
| imageId            | String             | &check;      |
| imageName          | String             | &check;      |
| memory             | String             | &check;      |
| name               | String             | &check;      |
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
