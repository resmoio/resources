---
description: Bitbucket Environment
---
bitbucket_environment
---------------------

| **Name**                 | **Type**           | **Nullable** |
| ------------------------ | ------------------ | ------------ |
| category                 | Map<String,String> | &check;      |
| deployment_gate_enabled  | Boolean            | &cross;      |
| environment_lock_enabled | Boolean            | &cross;      |
| environment_type         | EnvironmentType    | &check;      |
| hidden                   | Boolean            | &cross;      |
| lock                     | Lock               | &check;      |
| name                     | String             | &check;      |
| rank                     | Int                | &check;      |
| repository_id            | String             | &cross;      |
| restrictions             | Restrictions       | &check;      |
| slug                     | String             | &check;      |
| type                     | String             | &check;      |
| uuid                     | String             | &cross;      |
| workspace_id             | String             | &cross;      |

#### EnvironmentType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| rank     | Int      | &check;      |
| type     | String   | &check;      |

#### Lock
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Restrictions
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| admin_only | Boolean  | &check;      |
| type       | String   | &check;      |
