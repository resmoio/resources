---
description: GitHub Deployment
---
github_deployment
-----------------

| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| createdAt           | Date         | &check;      |
| creator             | User         | &check;      |
| description         | String       | &check;      |
| environment         | String       | &check;      |
| id                  | Long         | &cross;      |
| nodeId              | String       | &cross;      |
| organization        | Organization | &check;      |
| originalEnvironment | String       | &check;      |
| ref                 | String       | &check;      |
| repository          | Repository   | &check;      |
| sha                 | String       | &check;      |
| task                | String       | &check;      |
| updatedAt           | Date         | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### User
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |
