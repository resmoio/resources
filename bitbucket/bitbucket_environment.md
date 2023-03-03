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
| repository_name          | String             | &check;      |
| restrictions             | Restrictions       | &check;      |
| slug                     | String             | &check;      |
| type                     | String             | &check;      |
| uuid                     | String             | &cross;      |
| workspace_id             | String             | &cross;      |
| workspace_name           | String             | &check;      |

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
