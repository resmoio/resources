---
description: Entity Container
---
container
---------

| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| args           | List<String> | &check;      |
| command        | List<String> | &check;      |
| cpus           | String       | &check;      |
| id             | String       | &cross;      |
| imageId        | String       | &check;      |
| imageName      | String       | &check;      |
| memory         | String       | &check;      |
| name           | String       | &check;      |
| referencedType | String       | &cross;      |

#### BasicResource
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| referencedType | String   | &cross;      |
