---
description: Bitbucket Pipeline
---
bitbucket_pipeline
------------------

| **Name**           | **Type**   | **Nullable** |
| ------------------ | ---------- | ------------ |
| build_number       | Int        | &check;      |
| build_seconds_used | String     | &check;      |
| completed_on       | String     | &check;      |
| created_on         | String     | &check;      |
| creator            | Creator    | &check;      |
| repository         | Repository | &check;      |
| state              | State      | &check;      |
| target             | Target     | &check;      |
| trigger            | Trigger    | &check;      |
| uuid               | String     | &cross;      |
| workspace_id       | String     | &cross;      |

#### Creator
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| account_status  | String   | &check;      |
| created_on      | String   | &check;      |
| display_name    | String   | &check;      |
| has_2fa_enabled | Boolean  | &check;      |
| nickname        | String   | &check;      |
| type            | String   | &check;      |
| username        | String   | &check;      |
| uuid            | String   | &check;      |
| website         | String   | &check;      |

#### Repository
| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| created_on  | String             | &check;      |
| description | String             | &check;      |
| fork_policy | String             | &check;      |
| full_name   | String             | &check;      |
| has_issues  | Boolean            | &check;      |
| has_wiki    | Boolean            | &check;      |
| is_private  | Boolean            | &check;      |
| language    | String             | &check;      |
| mainbranch  | Repository.Branch  | &check;      |
| name        | String             | &check;      |
| owner       | Repository.Owner   | &cross;      |
| parent      | JSON               | &check;      |
| project     | Repository.Project | &check;      |
| scm         | String             | &check;      |
| size        | Int                | &check;      |
| updated_on  | String             | &check;      |
| uuid        | String             | &check;      |

#### Repository.Branch
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Repository.Owner
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_id   | String   | &check;      |
| display_name | String   | &check;      |
| type         | String   | &check;      |
| uuid         | String   | &check;      |

#### Repository.Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
| uuid     | String   | &check;      |

#### State
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| result   | JSON     | &check;      |
| type     | String   | &check;      |

#### Target
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### Trigger
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |
