---
description: Azure DevOps Deployment Group
---
azure_devops_deployment_group
-----------------------------

| **Name**     | **Type**      | **Nullable** |
| ------------ | ------------- | ------------ |
| accountId    | String        | &cross;      |
| accountName  | String        | &cross;      |
| description  | String        | &check;      |
| id           | String        | &cross;      |
| machineCount | Int           | &check;      |
| name         | String        | &check;      |
| pool         | TaskAgentPool | &check;      |
| project      | Project       | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### TaskAgentPool
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| isHosted | Boolean  | &check;      |
| isLegacy | Boolean  | &check;      |
| name     | String   | &check;      |
| options  | String   | &check;      |
| poolType | String   | &check;      |
| scope    | String   | &check;      |
