---
description: Firebase Ruleset
---
firebase_ruleset
----------------

| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| createTime | String       | &check;      |
| metadata   | MetadataInfo | &check;      |
| name       | String       | &cross;      |
| projectId  | String       | &cross;      |
| source     | Source       | &check;      |

#### MetadataInfo
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| services | List<String> | &check;      |

#### Source
| **Name** | **Type**          | **Nullable** |
| -------- | ----------------- | ------------ |
| files    | List<Source.File> | &check;      |

#### Source.File
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| content  | String   | &check;      |
| name     | String   | &check;      |
