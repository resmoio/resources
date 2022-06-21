---
description: GitHub Deploy Key
---
github_deploy_key
-----------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| createdAt    | Date         | &check;      |
| id           | Long         | &cross;      |
| key          | String       | &cross;      |
| organization | Organization | &check;      |
| readOnly     | Boolean      | &check;      |
| repository   | Repository   | &check;      |
| title        | String       | &check;      |
| verified     | Boolean      | &check;      |

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
