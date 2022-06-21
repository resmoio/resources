---
description: GitHub Repository
---
github_repo
-----------

| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| allowAutoMerge      | Boolean      | &check;      |
| allowMergeCommit    | Boolean      | &check;      |
| allowRebaseMerge    | Boolean      | &check;      |
| allowSquashMerge    | Boolean      | &check;      |
| archived            | Boolean      | &check;      |
| createdAt           | String       | &check;      |
| defaultBranch       | String       | &check;      |
| deleteBranchOnMerge | Boolean      | &check;      |
| description         | String       | &check;      |
| disabled            | Boolean      | &check;      |
| fork                | Boolean      | &check;      |
| forks               | Long         | &check;      |
| forksCount          | Long         | &check;      |
| fullName            | String       | &check;      |
| hasDownloads        | Boolean      | &check;      |
| hasIssues           | Boolean      | &check;      |
| hasPages            | Boolean      | &check;      |
| hasProjects         | Boolean      | &check;      |
| hasWiki             | Boolean      | &check;      |
| homepage            | String       | &check;      |
| id                  | Long         | &cross;      |
| isTemplate          | Boolean      | &check;      |
| language            | String       | &check;      |
| license             | License      | &check;      |
| name                | String       | &cross;      |
| networkCount        | Long         | &check;      |
| nodeId              | String       | &cross;      |
| openIssues          | Long         | &check;      |
| openIssuesCount     | Long         | &check;      |
| organization        | Organization | &check;      |
| parent              | Repo         | &check;      |
| permissions         | Permissions  | &check;      |
| private             | Boolean      | &check;      |
| source              | Repo         | &check;      |
| stargazersCount     | Long         | &check;      |
| subscribersCount    | Long         | &check;      |
| templateRepository  | Repo         | &check;      |
| topics              | List<String> | &check;      |
| updatedAt           | String       | &check;      |
| visibility          | String       | &check;      |
| watchers            | Long         | &check;      |
| watchersCount       | Long         | &check;      |

#### License
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| name     | String   | &check;      |
| nodeId   | String   | &check;      |
| spdxId   | String   | &check;      |
| url      | String   | &check;      |

#### Organization
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &cross;      |
| login     | String   | &cross;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Owner
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Permissions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| admin    | Boolean  | &check;      |
| pull     | Boolean  | &check;      |
| push     | Boolean  | &check;      |

#### Repo
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| fullName    | String   | &check;      |
| id          | Int      | &check;      |
| name        | String   | &check;      |
| nodeId      | String   | &check;      |
| owner       | Owner    | &check;      |
| private     | Boolean  | &check;      |
