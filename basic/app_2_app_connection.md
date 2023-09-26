---
description: Entity App-to-App Connection
---
app_2_app_connection
--------------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| active             | Boolean            | &cross;      |
| createdAt          | String             | &check;      |
| createdBy          | String             | &check;      |
| data               | JSON               | &check;      |
| destination        | Destination        | &cross;      |
| id                 | String             | &cross;      |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |
| source             | Source             | &cross;      |
| type               | String             | &cross;      |
| updatedAt          | String             | &check;      |

#### BasicResource
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |

#### ConnectionType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
| value    | String   | &cross;      |

#### Destination
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &cross;      |

#### ReferencedResource
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| groupKey      | String   | &cross;      |
| integrationId | String   | &cross;      |
| recordId      | String   | &cross;      |
| resourceId    | String   | &cross;      |
| resourceType  | String   | &cross;      |

#### Source
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
