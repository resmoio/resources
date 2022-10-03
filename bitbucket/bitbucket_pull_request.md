---
description: Bitbucket Pull Request
---
bitbucket_pull_request
----------------------

| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| author              | Account             | &check;      |
| close_source_branch | Boolean             | &cross;      |
| closed_by           | Account             | &check;      |
| comment_count       | Int                 | &check;      |
| created_on          | Date                | &check;      |
| destination         | PullRequestEndpoint | &check;      |
| id                  | String              | &cross;      |
| merge_commit        | Commit              | &check;      |
| participants        | List<Participant>   | &check;      |
| reason              | String              | &check;      |
| rendered            | JSON                | &check;      |
| reviewers           | List<Account>       | &check;      |
| source              | PullRequestEndpoint | &check;      |
| state               | String              | &check;      |
| summary             | JSON                | &check;      |
| task_count          | Int                 | &check;      |
| title               | String              | &check;      |
| updated_on          | Date                | &check;      |
| workspace_id        | String              | &cross;      |

#### Account
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| account_status  | String   | &check;      |
| has_2fa_enabled | Boolean  | &check;      |
| nickname        | String   | &check;      |
| username        | String   | &check;      |
| uuid            | String   | &check;      |

#### Commit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| hash     | String   | &check;      |

#### Participant
| **Name**        | **Type**         | **Nullable** |
| --------------- | ---------------- | ------------ |
| approved        | Boolean          | &cross;      |
| participated_on | Date             | &cross;      |
| role            | List<String>     | &cross;      |
| state           | String           | &cross;      |
| user            | Participant.User | &cross;      |

#### Participant.User
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| account_id   | String   | &check;      |
| display_name | String   | &check;      |
| nickname     | String   | &check;      |
| type         | String   | &check;      |
| uuid         | String   | &check;      |

#### PullRequestEndpoint
| **Name**   | **Type**                       | **Nullable** |
| ---------- | ------------------------------ | ------------ |
| branch     | PullRequestEndpoint.Branch     | &check;      |
| commit     | Commit                         | &check;      |
| repository | PullRequestEndpoint.Repository | &check;      |

#### PullRequestEndpoint.Branch
| **Name** | **Type**                          | **Nullable** |
| -------- | --------------------------------- | ------------ |
| name     | String                            | &check;      |
| target   | PullRequestEndpoint.Branch.Target | &check;      |
| type     | String                            | &check;      |

#### PullRequestEndpoint.Branch.Target
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| hash     | String   | &check;      |

#### PullRequestEndpoint.Repository
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| full_name | String   | &check;      |
| name      | String   | &check;      |
| type      | String   | &check;      |
| uuid      | String   | &check;      |
