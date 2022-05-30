---
description: Bitbucket Workspace User
---
bitbucket_workspace_user
------------------------

| **Name**   | **Type**  | **Nullable** |
| ---------- | --------- | ------------ |
| permission | String    | &cross;      |
| user       | Account   | &cross;      |
| workspace  | Workspace | &cross;      |

#### Account
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| account_status  | String   | &check;      |
| has_2fa_enabled | Boolean  | &check;      |
| nickname        | String   | &check;      |
| username        | String   | &check;      |
| uuid            | String   | &cross;      |

#### Workspace
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| slug     | String   | &check;      |
| type     | String   | &check;      |
| uuid     | String   | &cross;      |
