---
description: Snyk Project
---
snyk_project
------------

| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| branch                | String                | &check;      |
| created               | String                | &check;      |
| id                    | String                | &cross;      |
| imageId               | String                | &check;      |
| imageTag              | String                | &check;      |
| importingUser         | ImportingUser         | &check;      |
| isMonitored           | Boolean               | &check;      |
| issueCountsBySeverity | IssueCountsBySeverity | &check;      |
| lastTestedDate        | String                | &check;      |
| name                  | String                | &check;      |
| orgId                 | String                | &check;      |
| orgName               | String                | &check;      |
| origin                | String                | &check;      |
| owner                 | Owner                 | &check;      |
| readOnly              | Boolean               | &check;      |
| remoteRepoUrl         | String                | &check;      |
| settings              | Settings              | &check;      |
| tags                  | List<Tag>             | &check;      |
| testFrequency         | String                | &check;      |
| totalDependencies     | Int                   | &check;      |
| type                  | String                | &check;      |

#### AutoRemediationPrs
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| backlogPrsEnabled   | Boolean  | &check;      |
| freshPrsEnabled     | Boolean  | &check;      |
| usePatchRemediation | Boolean  | &check;      |

#### ImportingUser
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |
| name     | String   | &check;      |
| username | String   | &check;      |

#### IssueCountsBySeverity
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| critical | Int      | &check;      |
| high     | Int      | &check;      |
| low      | Int      | &check;      |
| medium   | Int      | &check;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |
| name     | String   | &check;      |
| username | String   | &check;      |

#### PullRequestAssignment
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| assignees | List<String> | &check;      |
| enabled   | Boolean      | &check;      |
| type      | String       | &check;      |

#### Settings
| **Name**                           | **Type**              | **Nullable** |
| ---------------------------------- | --------------------- | ------------ |
| autoDepUpgradeEnabled              | Boolean               | &check;      |
| autoDepUpgradeIgnoredDependencies  | List<String>          | &check;      |
| autoDepUpgradeLimit                | Int                   | &check;      |
| autoDepUpgradeMinAge               | Int                   | &check;      |
| autoRemediationPrs                 | AutoRemediationPrs    | &check;      |
| pullRequestAssignment              | PullRequestAssignment | &check;      |
| pullRequestFailOnAnyVulns          | Boolean               | &check;      |
| pullRequestFailOnlyForHighSeverity | Boolean               | &check;      |
| pullRequestTestEnabled             | Boolean               | &check;      |

#### Tag
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| value    | String   | &check;      |
