---
description: Azure DevOps Project
---
azure_devops_project
--------------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| accountId      | String         | &cross;      |
| accountName    | String         | &cross;      |
| description    | String         | &check;      |
| id             | String         | &cross;      |
| lastUpdateTime | String         | &check;      |
| name           | String         | &cross;      |
| properties     | List<Property> | &check;      |
| revision       | Int            | &check;      |
| state          | String         | &check;      |
| url            | String         | &check;      |
| visibility     | String         | &check;      |

#### Property
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |
