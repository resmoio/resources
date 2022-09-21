---
description: Azure DevOps Pipeline Run
---
azure_devops_pipeline_run
-------------------------

| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| accountId    | String   | &cross;      |
| accountName  | String   | &cross;      |
| createdDate  | String   | &check;      |
| finalYaml    | String   | &check;      |
| finishedDate | String   | &check;      |
| id           | String   | &cross;      |
| name         | String   | &cross;      |
| pipeline     | Pipeline | &check;      |
| projectId    | String   | &cross;      |
| resources    | JSON     | &check;      |
| result       | String   | &check;      |
| state        | String   | &check;      |
| url          | String   | &check;      |
| variables    | JSON     | &check;      |

#### Pipeline
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| folder   | String   | &check;      |
| id       | String   | &check;      |
| name     | String   | &check;      |
| revision | Int      | &check;      |
| url      | String   | &check;      |
