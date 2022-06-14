---
description: Bitbucket Repository
---
bitbucket_repository
--------------------

| **Name**          | **Type**         | **Nullable** |
| ----------------- | ---------------- | ------------ |
| created_on        | String           | &check;      |
| description       | String           | &check;      |
| fork_policy       | String           | &check;      |
| full_name         | String           | &check;      |
| has_issues        | Boolean          | &check;      |
| has_wiki          | Boolean          | &check;      |
| is_private        | Boolean          | &cross;      |
| mainbranch        | MainBranch       | &check;      |
| override_settings | OverrideSettings | &check;      |
| owner             | Owner            | &cross;      |
| project           | Project          | &check;      |
| scm               | String           | &check;      |
| slug              | String           | &check;      |
| type              | String           | &check;      |
| uuid              | String           | &cross;      |
| website           | String           | &check;      |
| workspace         | Workspace        | &cross;      |

#### MainBranch
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### OverrideSettings
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| branching_model        | Boolean  | &check;      |
| default_merge_strategy | Boolean  | &check;      |

#### Owner
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_id   | String   | &check;      |
| display_name | String   | &check;      |
| type         | String   | &check;      |
| uuid         | String   | &cross;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
| uuid     | String   | &check;      |

#### Workspace
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| slug     | String   | &check;      |
| type     | String   | &check;      |
| uuid     | String   | &cross;      |
