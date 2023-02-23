---
description: Entity DNS Record
---
dns_record
----------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| domain             | String             | &cross;      |
| name               | String             | &cross;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |
| ttl                | Long               | &check;      |
| type               | String             | &cross;      |
| value              | String             | &cross;      |

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
