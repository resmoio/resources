---
description: Entity Domain
---
domain
------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| abuseContactEmail  | String             | &check;      |
| autoRenew          | Boolean            | &check;      |
| contactEmails      | List<String>       | &check;      |
| id                 | String             | &cross;      |
| locked             | Boolean            | &check;      |
| name               | String             | &check;      |
| nameServers        | List<String>       | &check;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |
| registrar          | String             | &check;      |
| tld                | String             | &check;      |

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
