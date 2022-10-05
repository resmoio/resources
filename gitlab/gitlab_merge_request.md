---
description: GitLab Merge Request
---
gitlab_merge_request
--------------------

| **Name**                    | **Type**             | **Nullable** |
| --------------------------- | -------------------- | ------------ |
| approvalsBeforeMerge        | String               | &check;      |
| assignee                    | User                 | &check;      |
| assignees                   | List<User>           | &check;      |
| author                      | User                 | &check;      |
| blockingDiscussionsResolved | Boolean              | &check;      |
| closedAt                    | Date                 | &check;      |
| closedBy                    | User                 | &check;      |
| createdAt                   | Date                 | &check;      |
| description                 | String               | &check;      |
| discussionLocked            | String               | &check;      |
| downvotes                   | Int                  | &check;      |
| draft                       | Boolean              | &check;      |
| forceRemoveSourceBranch     | Boolean              | &check;      |
| hasConflicts                | Boolean              | &check;      |
| id                          | String               | &cross;      |
| iid                         | Int                  | &check;      |
| labels                      | List<String>         | &check;      |
| mergeCommitSha              | String               | &check;      |
| mergeStatus                 | String               | &check;      |
| mergeWhenPipelineSucceeds   | Boolean              | &check;      |
| mergedAt                    | Date                 | &check;      |
| mergedBy                    | User                 | &check;      |
| milestone                   | Milestone            | &check;      |
| projectId                   | Int                  | &check;      |
| reference                   | String               | &check;      |
| references                  | References           | &check;      |
| reviewers                   | List<User>           | &check;      |
| sha                         | String               | &check;      |
| shouldRemoveSourceBranch    | String               | &check;      |
| sourceBranch                | String               | &check;      |
| sourceProjectId             | Int                  | &check;      |
| squash                      | Boolean              | &check;      |
| squashCommitSha             | String               | &check;      |
| state                       | String               | &check;      |
| targetBranch                | String               | &check;      |
| targetProjectId             | Int                  | &check;      |
| taskCompletionStatus        | TaskCompletionStatus | &check;      |
| timeStats                   | TimeStats            | &check;      |
| title                       | String               | &check;      |
| updatedAt                   | Date                 | &check;      |
| upvotes                     | Int                  | &check;      |
| userNotesCount              | Int                  | &check;      |
| webUrl                      | String               | &check;      |
| workInProgress              | Boolean              | &check;      |

#### Milestone
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| createdAt   | Date     | &check;      |
| description | String   | &check;      |
| dueDate     | Date     | &check;      |
| expired     | Boolean  | &check;      |
| groupId     | Long     | &check;      |
| id          | Long     | &check;      |
| iid         | Long     | &check;      |
| startDate   | Date     | &check;      |
| state       | String   | &check;      |
| title       | String   | &check;      |
| updatedAt   | Date     | &check;      |
| webUrl      | String   | &check;      |

#### References
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| full     | String   | &check;      |
| relative | String   | &check;      |
| short    | String   | &check;      |

#### TaskCompletionStatus
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| completedCount | Int      | &check;      |
| count          | Int      | &check;      |

#### TimeStats
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| humanTimeEstimate   | String   | &check;      |
| humanTotalTimeSpent | String   | &check;      |
| timeEstimate        | Int      | &check;      |
| totalTimeSpent      | Int      | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| state    | String   | &check;      |
| username | String   | &check;      |
