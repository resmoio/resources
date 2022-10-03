---
description: Bitbucket Deployment
---
bitbucket_deployment
--------------------

| **Name**         | **Type**    | **Nullable** |
| ---------------- | ----------- | ------------ |
| deployable       | JSON        | &cross;      |
| environment      | Environment | &check;      |
| key              | String      | &check;      |
| last_update_time | Date        | &check;      |
| number           | Int         | &check;      |
| release          | Release     | &check;      |
| repository_id    | String      | &cross;      |
| state            | State       | &check;      |
| step             | Step        | &check;      |
| type             | String      | &check;      |
| uuid             | String      | &cross;      |
| version          | Int         | &check;      |
| workspace_id     | String      | &cross;      |

#### Commit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| hash     | String   | &check;      |

#### Environment
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| uuid     | String   | &check;      |

#### Release
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| commit     | Commit   | &check;      |
| created_on | String   | &check;      |
| type       | String   | &check;      |
| uuid       | String   | &check;      |

#### State
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| completed_on               | String   | &check;      |
| last_successful_deployment | JSON     | &check;      |
| name                       | String   | &check;      |
| started_on                 | String   | &check;      |
| status                     | Status   | &check;      |
| type                       | String   | &check;      |
| url                        | String   | &check;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Step
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| uuid     | String   | &check;      |
