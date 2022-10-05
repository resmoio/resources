---
description: Azure DevOps Pull Request
---
azure_devops_pullrequest
------------------------

| **Name**              | **Type**          | **Nullable** |
| --------------------- | ----------------- | ------------ |
| accountId             | String            | &cross;      |
| accountName           | String            | &cross;      |
| artifactId            | String            | &check;      |
| autoCompleteSetBy     | Identity          | &check;      |
| closedBy              | Identity          | &check;      |
| closedDate            | Date              | &check;      |
| codeReviewId          | Int               | &check;      |
| commits               | List<Commit>      | &check;      |
| completionOptions     | CompletionOptions | &check;      |
| completionQueueTime   | String            | &check;      |
| createdBy             | Identity          | &check;      |
| creationDate          | Date              | &check;      |
| description           | String            | &check;      |
| forkSource            | Fork              | &check;      |
| hasMultipleMergeBases | Boolean           | &check;      |
| isDraft               | Boolean           | &check;      |
| labels                | List<Label>       | &check;      |
| lastMergeCommit       | Commit            | &check;      |
| lastMergeSourceCommit | Commit            | &check;      |
| lastMergeTargetCommit | Commit            | &check;      |
| mergeFailureMessage   | String            | &check;      |
| mergeFailureType      | String            | &check;      |
| mergeId               | String            | &check;      |
| mergeOptions          | MergeOptions      | &check;      |
| mergeStatus           | String            | &check;      |
| projectId             | String            | &cross;      |
| pullRequestId         | String            | &cross;      |
| remoteUrl             | String            | &check;      |
| repository            | Repository        | &check;      |
| reviewers             | List<Reviewer>    | &check;      |
| sourceRefName         | String            | &check;      |
| status                | String            | &check;      |
| supportsIterations    | Boolean           | &check;      |
| targetRefName         | String            | &check;      |
| title                 | String            | &check;      |
| url                   | String            | &check;      |

#### Commit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| commitId | String   | &check;      |
| url      | String   | &check;      |

#### CompletionOptions
| **Name**                    | **Type**  | **Nullable** |
| --------------------------- | --------- | ------------ |
| autoCompleteIgnoreConfigIds | List<Int> | &check;      |
| bypassPolicy                | Boolean   | &check;      |
| bypassReason                | String    | &check;      |
| deleteSourceBranch          | Boolean   | &check;      |
| mergeCommitMessage          | String    | &check;      |
| mergeStrategy               | String    | &check;      |
| transitionWorkItems         | Boolean   | &check;      |
| triggeredByAutoComplete     | Boolean   | &check;      |

#### Fork
| **Name**       | **Type**   | **Nullable** |
| -------------- | ---------- | ------------ |
| creator        | Identity   | &check;      |
| isLocked       | Boolean    | &check;      |
| isLockedBy     | Identity   | &check;      |
| name           | String     | &check;      |
| objectId       | String     | &check;      |
| peeledObjectId | String     | &check;      |
| repository     | Repository | &check;      |
| statuses       | JSON       | &check;      |
| url            | String     | &check;      |

#### Identity
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| displayName       | String   | &check;      |
| id                | String   | &check;      |
| imageUrl          | String   | &check;      |
| isAadIdentity     | Boolean  | &check;      |
| isContainer       | Boolean  | &check;      |
| isDeletedInOrigin | Boolean  | &check;      |
| profileUrl        | String   | &check;      |
| uniqueName        | String   | &check;      |
| url               | String   | &check;      |

#### Label
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| active   | Boolean  | &check;      |
| id       | String   | &check;      |
| name     | String   | &check;      |
| url      | String   | &check;      |

#### MergeOptions
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| conflictAuthorshipCommits  | Boolean  | &check;      |
| detectRenameFalsePositives | Boolean  | &check;      |
| disableRenames             | Boolean  | &check;      |

#### Repository
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| id       | String             | &check;      |
| name     | String             | &check;      |
| project  | Repository.Project | &check;      |
| url      | String             | &check;      |

#### Repository.Project
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| id             | String   | &check;      |
| lastUpdateTime | Date     | &check;      |
| name           | String   | &check;      |
| state          | String   | &check;      |
| visibility     | String   | &check;      |

#### Reviewer
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| hasDeclined | Boolean  | &check;      |
| id          | String   | &check;      |
| imageUrl    | String   | &check;      |
| isFlagged   | Boolean  | &check;      |
| isRequired  | Boolean  | &check;      |
| reviewerUrl | String   | &check;      |
| uniqueName  | String   | &check;      |
| vote        | Int      | &check;      |
