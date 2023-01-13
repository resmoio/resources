---
description: GitHub App Installation
---
github_app_installation
-----------------------

| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| account                | Account      | &check;      |
| appId                  | Long         | &check;      |
| appSlug                | String       | &check;      |
| createdAt              | String       | &check;      |
| events                 | List<String> | &check;      |
| hasMultipleSingleFiles | Boolean      | &check;      |
| id                     | Long         | &cross;      |
| organization           | Organization | &check;      |
| permissions            | Permissions  | &check;      |
| repositorySelection    | String       | &check;      |
| singleFileName         | String       | &check;      |
| singleFilePaths        | List<String> | &check;      |
| suspendedAt            | String       | &check;      |
| suspendedBy            | String       | &check;      |
| targetId               | Long         | &check;      |
| targetType             | String       | &check;      |
| updatedAt              | String       | &check;      |

#### Account
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### Permissions
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| checks             | String   | &check;      |
| contents           | String   | &check;      |
| deployments        | String   | &check;      |
| discussions        | String   | &check;      |
| issues             | String   | &check;      |
| metadata           | String   | &check;      |
| pullRequests       | String   | &check;      |
| repositoryProjects | String   | &check;      |
| statuses           | String   | &check;      |
