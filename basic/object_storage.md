---
description: Entity Object Storage
---
object_storage
--------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| backupEnabled      | Boolean            | &check;      |
| backupRetention    | Long               | &check;      |
| encrypted          | Boolean            | &check;      |
| isEu               | Boolean            | &check;      |
| name               | String             | &cross;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |
| region             | String             | &check;      |

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
