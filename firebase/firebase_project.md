---
description: Firebase Project
---
firebase_project
----------------

| **Name**      | **Type**        | **Nullable** |
| ------------- | --------------- | ------------ |
| displayName   | String          | &check;      |
| etag          | String          | &check;      |
| name          | String          | &check;      |
| projectId     | String          | &cross;      |
| projectNumber | String          | &cross;      |
| releases      | List<Release>   | &check;      |
| resources     | ProjectResource | &check;      |
| services      | List<Service>   | &check;      |
| state         | String          | &check;      |

#### ProjectResource
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| hostingSite              | String   | &check;      |
| locationId               | String   | &check;      |
| realtimeDatabaseInstance | String   | &check;      |
| storageBucket            | String   | &check;      |

#### Release
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| createTime  | String   | &check;      |
| name        | String   | &check;      |
| rulesetName | String   | &check;      |
| updateTime  | String   | &check;      |

#### Service
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| enforcementMode | String   | &check;      |
| name            | String   | &check;      |
