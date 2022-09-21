---
description: Azure DevOps Pipeline
---
azure_devops_pipeline
---------------------

| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| accountId     | String        | &cross;      |
| accountName   | String        | &cross;      |
| configuration | Configuration | &check;      |
| folder        | String        | &check;      |
| id            | String        | &cross;      |
| name          | String        | &check;      |
| projectId     | String        | &cross;      |
| revision      | Int           | &check;      |
| url           | String        | &check;      |

#### Configuration
| **Name**   | **Type**                 | **Nullable** |
| ---------- | ------------------------ | ------------ |
| path       | String                   | &check;      |
| repository | Configuration.Repository | &check;      |
| type       | String                   | &check;      |

#### Configuration.Repository
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| type     | String   | &check;      |
