---
description: GitHub Deployment Environment
---
github_deployment_env
---------------------

| **Name**               | **Type**               | **Nullable** |
| ---------------------- | ---------------------- | ------------ |
| createdAt              | Date                   | &check;      |
| deploymentBranchPolicy | DeploymentBranchPolicy | &check;      |
| id                     | Long                   | &cross;      |
| name                   | String                 | &cross;      |
| nodeId                 | String                 | &cross;      |
| organizationId         | String                 | &cross;      |
| protectionRules        | List<ProtectionRule>   | &check;      |
| repositoryId           | String                 | &cross;      |
| updatedAt              | Date                   | &check;      |

#### DeploymentBranchPolicy
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| customBranchPolicies | Boolean  | &check;      |
| protectedBranches    | Boolean  | &check;      |

#### ProtectionRule
| **Name**  | **Type**        | **Nullable** |
| --------- | --------------- | ------------ |
| id        | Long            | &cross;      |
| nodeId    | String          | &cross;      |
| reviewers | List<Reviewers> | &check;      |
| type      | String          | &cross;      |
| waitTimer | Int             | &check;      |

#### Reviewer
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| id          | Long     | &cross;      |
| login       | String   | &check;      |
| name        | String   | &check;      |
| nodeId      | String   | &cross;      |
| permission  | String   | &check;      |
| privacy     | String   | &check;      |
| siteAdmin   | Boolean  | &check;      |
| slug        | String   | &check;      |
| type        | String   | &check;      |

#### Reviewers
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| reviewer | Reviewer | &check;      |
| type     | String   | &cross;      |
