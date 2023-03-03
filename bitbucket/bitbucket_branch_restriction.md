---
description: Bitbucket Branch Restriction
---
bitbucket_branch_restriction
----------------------------

| **Name**          | **Type**      | **Nullable** |
| ----------------- | ------------- | ------------ |
| branch_match_kind | String        | &check;      |
| branch_type       | String        | &check;      |
| groups            | List<Group>   | &check;      |
| id                | Int           | &cross;      |
| kind              | String        | &check;      |
| pattern           | String        | &check;      |
| repository_id     | String        | &cross;      |
| repository_name   | String        | &check;      |
| users             | List<Account> | &check;      |
| value             | Int           | &check;      |
| workspace_id      | String        | &check;      |
| workspace_name    | String        | &check;      |

#### Account
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| account_status  | String   | &check;      |
| has_2fa_enabled | Boolean  | &check;      |
| nickname        | String   | &check;      |
| username        | String   | &check;      |
| uuid            | String   | &check;      |

#### Group
| **Name**  | **Type**        | **Nullable** |
| --------- | --------------- | ------------ |
| full_slug | String          | &check;      |
| name      | String          | &check;      |
| owner     | Group.Owner     | &check;      |
| slug      | String          | &check;      |
| workspace | Group.Workspace | &check;      |

#### Group.Owner
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_id   | String   | &check;      |
| display_name | String   | &check;      |
| type         | String   | &check;      |
| uuid         | String   | &check;      |

#### Group.Workspace
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| slug     | String   | &check;      |
| type     | String   | &check;      |
| uuid     | String   | &check;      |
