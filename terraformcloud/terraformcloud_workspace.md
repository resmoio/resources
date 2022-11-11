---
description: Terraform Cloud Workspace
---
terraformcloud_workspace
------------------------

| **Name**             | **Type**            | **Nullable** |
| -------------------- | ------------------- | ------------ |
| actions              | Map<String,Boolean> | &check;      |
| allowDestroyPlan     | Boolean             | &check;      |
| applyDurationAverage | String              | &check;      |
| autoApply            | Boolean             | &check;      |
| autoDestroyAt        | String              | &check;      |
| createdAt            | String              | &check;      |
| description          | String              | &check;      |
| environment          | String              | &check;      |
| executionMode        | String              | &check;      |
| fileTriggersEnabled  | Boolean             | &check;      |
| globalRemoteState    | Boolean             | &check;      |
| id                   | String              | &cross;      |
| latestChangeAt       | String              | &check;      |
| locked               | Boolean             | &check;      |
| name                 | String              | &check;      |
| operations           | Boolean             | &check;      |
| organization         | String              | &check;      |
| permissions          | Map<String,Boolean> | &check;      |
| type                 | String              | &check;      |
| updatedAt            | String              | &check;      |
| vcsRepo              | VcsRepo             | &check;      |

#### VcsRepo
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| identifier      | String   | &check;      |
| serviceProvider | String   | &check;      |
