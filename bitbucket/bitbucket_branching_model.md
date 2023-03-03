---
description: Bitbucket Branching Model
---
bitbucket_branching_model
-------------------------

| **Name**        | **Type**         | **Nullable** |
| --------------- | ---------------- | ------------ |
| branch_types    | List<BranchType> | &check;      |
| development     | Development      | &cross;      |
| production      | Production       | &check;      |
| repository_id   | String           | &cross;      |
| repository_name | String           | &check;      |
| type            | String           | &check;      |
| workspace_id    | String           | &check;      |
| workspace_name  | String           | &check;      |

#### Branch
| **Name** | **Type**      | **Nullable** |
| -------- | ------------- | ------------ |
| name     | String        | &check;      |
| target   | Branch.Target | &check;      |
| type     | String        | &check;      |

#### Branch.Target
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| hash     | String   | &check;      |

#### BranchType
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| kind     | String   | &check;      |
| prefix   | String   | &check;      |

#### Development
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| branch         | Branch   | &check;      |
| name           | String   | &check;      |
| use_mainbranch | Boolean  | &check;      |

#### Production
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| branch         | Branch   | &check;      |
| name           | String   | &check;      |
| use_mainbranch | Boolean  | &check;      |
