---
description: Segment Source
---
segment_source
--------------

| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| enabled     | Boolean            | &check;      |
| id          | String             | &cross;      |
| labels      | List<Label>        | &check;      |
| metadata    | Metadata           | &check;      |
| name        | String             | &check;      |
| settings    | Map<String,String> | &check;      |
| slug        | String             | &check;      |
| workspaceId | String             | &check;      |

#### Label
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| key         | String   | &check;      |
| value       | String   | &check;      |

#### Logos
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| alt      | String   | &check;      |
| default  | String   | &check;      |
| mark     | String   | &check;      |

#### Metadata
| **Name**           | **Type**      | **Nullable** |
| ------------------ | ------------- | ------------ |
| categories         | List<String>  | &check;      |
| description        | String        | &check;      |
| id                 | String        | &check;      |
| isCloudEventSource | Boolean       | &check;      |
| logos              | Logos         | &check;      |
| name               | String        | &check;      |
| options            | List<Options> | &check;      |
| slug               | String        | &check;      |

#### Options
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| defaultValue | String   | &check;      |
| description  | String   | &check;      |
| label        | String   | &check;      |
| name         | String   | &check;      |
| required     | Boolean  | &check;      |
| type         | String   | &check;      |
