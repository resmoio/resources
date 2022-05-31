---
description: GitHub Deployment
---
github_deployment
-----------------

| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| createdAt           | Date     | &check;      |
| creator             | User     | &check;      |
| description         | String   | &check;      |
| environment         | String   | &check;      |
| id                  | Long     | &cross;      |
| nodeId              | String   | &cross;      |
| organizationId      | String   | &cross;      |
| originalEnvironment | String   | &check;      |
| ref                 | String   | &check;      |
| repositoryId        | String   | &cross;      |
| sha                 | String   | &check;      |
| task                | String   | &check;      |
| updatedAt           | Date     | &check;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
