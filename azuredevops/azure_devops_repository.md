---
description: Azure DevOps Repository
---
azure_devops_repository
-----------------------

| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| accountId        | String           | &cross;      |
| accountName      | String           | &cross;      |
| defaultBranch    | String           | &check;      |
| id               | String           | &cross;      |
| isFork           | Boolean          | &check;      |
| name             | String           | &check;      |
| parentRepository | ParentRepository | &check;      |
| project          | Project          | &check;      |
| remoteUrl        | String           | &check;      |
| sshUrl           | String           | &check;      |
| url              | String           | &check;      |
| validRemoteUrls  | List<String>     | &check;      |
| webUrl           | String           | &check;      |

#### ParentRepository
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| isFork    | Boolean  | &check;      |
| name      | String   | &check;      |
| project   | Project  | &cross;      |
| remoteUrl | String   | &check;      |
| sshUrl    | String   | &check;      |
| url       | String   | &check;      |

#### Project
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| accountName    | String   | &check;      |
| description    | String   | &check;      |
| id             | String   | &check;      |
| lastUpdateTime | String   | &check;      |
| name           | String   | &check;      |
| revision       | Int      | &check;      |
| state          | String   | &check;      |
| url            | String   | &check;      |
| visibility     | String   | &check;      |
