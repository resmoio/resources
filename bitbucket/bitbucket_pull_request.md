---
description: Bitbucket Pull Request
---
bitbucket_pull_request
----------------------

| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| author              | Account             | &check;      |
| close_source_branch | Boolean             | &check;      |
| closed_by           | Account             | &check;      |
| comment_count       | Int                 | &check;      |
| created_on          | Date                | &check;      |
| destination         | PullRequestEndpoint | &check;      |
| id                  | String              | &cross;      |
| merge_commit        | Commit              | &check;      |
| reason              | String              | &check;      |
| source              | PullRequestEndpoint | &check;      |
| state               | String              | &check;      |
| summary             | JSON                | &check;      |
| task_count          | Int                 | &check;      |
| title               | String              | &check;      |
| updated_on          | Date                | &check;      |
| workspace_id        | String              | &cross;      |

#### Account
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| nickname | String   | &check;      |
| uuid     | String   | &check;      |

#### Commit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| hash     | String   | &check;      |

#### PullRequestEndpoint
| **Name**   | **Type**                       | **Nullable** |
| ---------- | ------------------------------ | ------------ |
| branch     | PullRequestEndpoint.Branch     | &check;      |
| commit     | Commit                         | &check;      |
| repository | PullRequestEndpoint.Repository | &check;      |

#### PullRequestEndpoint.Branch
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |

#### PullRequestEndpoint.Repository
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| full_name | String   | &check;      |
| name      | String   | &check;      |
| type      | String   | &check;      |
| uuid      | String   | &check;      |
