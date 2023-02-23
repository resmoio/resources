---
description: Entity IP Address
---
ip_address
----------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| dnsName            | String             | &check;      |
| id                 | String             | &cross;      |
| ip                 | String             | &check;      |
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
