---
description: GitHub Actions Workflow Run
---
github_actions_workflow_run
---------------------------

| **Name**         | **Type**          | **Nullable** |
| ---------------- | ----------------- | ------------ |
| actor            | Actor             | &check;      |
| checkSuiteId     | Long              | &check;      |
| checkSuiteNodeId | String            | &check;      |
| conclusion       | String            | &check;      |
| createdAt        | String            | &check;      |
| event            | String            | &check;      |
| headBranch       | String            | &check;      |
| headCommit       | HeadCommit        | &check;      |
| headRepository   | Repository        | &check;      |
| headSha          | String            | &check;      |
| id               | Long              | &cross;      |
| name             | String            | &check;      |
| nodeId           | String            | &check;      |
| organization     | Organization      | &cross;      |
| pullRequests     | List<PullRequest> | &check;      |
| repository       | Repository        | &cross;      |
| runAttempt       | Long              | &check;      |
| runNumber        | Long              | &check;      |
| runStartedAt     | String            | &check;      |
| status           | String            | &check;      |
| triggeringActor  | Actor             | &check;      |
| updatedAt        | String            | &check;      |
| workflowId       | Long              | &check;      |
| workflowUrl      | String            | &check;      |

#### Actor
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| gravatarId | String   | &check;      |
| id         | Int      | &cross;      |
| login      | String   | &cross;      |
| nodeId     | String   | &check;      |
| siteAdmin  | Boolean  | &check;      |
| type       | String   | &check;      |

#### HeadCommit
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| author    | Member   | &check;      |
| committer | Member   | &check;      |
| id        | String   | &check;      |
| message   | String   | &check;      |
| timestamp | String   | &check;      |
| treeId    | String   | &check;      |

#### Member
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| name     | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### PullRequest
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |

#### Repository
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| fork        | Boolean  | &check;      |
| fullName    | String   | &check;      |
| id          | Long     | &cross;      |
| name        | String   | &cross;      |
| nodeId      | String   | &check;      |
| owner       | Actor    | &check;      |
| private     | Boolean  | &check;      |
