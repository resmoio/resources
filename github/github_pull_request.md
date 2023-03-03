---
description: GitHub Pull Request
---
github_pull_request
-------------------

| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| activeLockReason    | String              | &check;      |
| additions           | Long                | &check;      |
| assignees           | List<User>          | &check;      |
| authorAssociation   | String              | &check;      |
| autoMerge           | AutoMerge           | &check;      |
| base                | Base                | &check;      |
| body                | String              | &check;      |
| changedFiles        | Long                | &check;      |
| closedAt            | Date                | &check;      |
| comments            | Long                | &check;      |
| commits             | Long                | &check;      |
| createdAt           | Date                | &check;      |
| deletions           | Long                | &check;      |
| draft               | Boolean             | &check;      |
| head                | Head                | &check;      |
| id                  | Long                | &cross;      |
| labels              | List<Label>         | &check;      |
| locked              | Boolean             | &check;      |
| maintainerCanModify | Boolean             | &check;      |
| mergeCommitSha      | String              | &check;      |
| mergeable           | Boolean             | &check;      |
| mergeableState      | String              | &check;      |
| merged              | Boolean             | &check;      |
| mergedAt            | Date                | &check;      |
| mergedBy            | User                | &check;      |
| milestone           | Milestone           | &check;      |
| nodeId              | String              | &cross;      |
| number              | Long                | &cross;      |
| organization        | Organization        | &check;      |
| rebaseable          | Boolean             | &check;      |
| repository          | Repository          | &check;      |
| requestedReviewers  | List<User>          | &check;      |
| requestedTeams      | List<RequestedTeam> | &check;      |
| reviewComments      | Long                | &check;      |
| state               | String              | &check;      |
| title               | String              | &check;      |
| updatedAt           | Date                | &check;      |
| user                | User                | &check;      |

#### AutoMerge
| **Name**      | **Type**  | **Nullable** |
| ------------- | --------- | ------------ |
| commitMessage | String    | &check;      |
| commitTitle   | String    | &check;      |
| enabledBy     | EnabledBy | &check;      |
| mergeMethod   | String    | &check;      |

#### Base
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| label    | String   | &check;      |
| ref      | String   | &check;      |
| repo     | Repo     | &check;      |
| sha      | String   | &check;      |
| user     | User     | &check;      |

#### EnabledBy
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Int      | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Head
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| label    | String   | &check;      |
| ref      | String   | &check;      |
| repo     | Repo     | &check;      |
| sha      | String   | &check;      |
| user     | User     | &check;      |

#### Label
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| color       | String   | &check;      |
| default     | Boolean  | &check;      |
| description | String   | &check;      |
| name        | String   | &cross;      |
| nodeId      | String   | &cross;      |

#### License
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| name     | String   | &check;      |
| nodeId   | String   | &check;      |
| spdxId   | String   | &check;      |
| url      | String   | &check;      |

#### Milestone
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| closedAt     | Date     | &check;      |
| closedIssues | Long     | &check;      |
| createdAt    | Date     | &check;      |
| creator      | User     | &check;      |
| description  | String   | &check;      |
| dueOn        | Date     | &check;      |
| nodeId       | String   | &cross;      |
| number       | Long     | &cross;      |
| openIssues   | Long     | &check;      |
| state        | String   | &check;      |
| title        | String   | &check;      |
| updatedAt    | Date     | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Owner
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Repo
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| fullName    | String   | &check;      |
| id          | Long     | &check;      |
| name        | String   | &check;      |
| nodeId      | String   | &check;      |
| owner       | Owner    | &check;      |
| private     | Boolean  | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### RequestedTeam
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | Long     | &cross;      |
| name        | String   | &cross;      |
| nodeId      | String   | &cross;      |
| privacy     | String   | &check;      |
| slug        | String   | &check;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
