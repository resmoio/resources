---
description: Drata Workspace
---
drata_workspace
---------------

| **Name**    | **Type**        | **Nullable** |
| ----------- | --------------- | ------------ |
| description | String          | &check;      |
| frameworks  | List<Framework> | &check;      |
| howItWorks  | String          | &check;      |
| id          | Long            | &cross;      |
| name        | String          | &check;      |
| primary     | Boolean         | &check;      |
| url         | String          | &check;      |

#### Framework
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| controlsEnabled             | Boolean  | &check;      |
| createdAt                   | String   | &check;      |
| customFrameworkId           | String   | &check;      |
| description                 | String   | &check;      |
| enabledAt                   | String   | &check;      |
| frameworkEnabled            | Boolean  | &check;      |
| hasLevel                    | Boolean  | &check;      |
| id                          | Long     | &check;      |
| isReady                     | Boolean  | &check;      |
| label                       | String   | &check;      |
| levelLabel                  | String   | &check;      |
| longDescription             | String   | &check;      |
| name                        | String   | &check;      |
| numInScopeRequirements      | Long     | &check;      |
| numReadyInScopeRequirements | Long     | &check;      |
| privacy                     | Boolean  | &check;      |
| productFrameworkEnabled     | Boolean  | &check;      |
| selectedLevel               | String   | &check;      |
| slug                        | String   | &check;      |
| tag                         | String   | &check;      |
| totalEnabledControls        | Long     | &check;      |
| totalInScopeControls        | Long     | &check;      |
| type                        | String   | &check;      |
| updatedAt                   | String   | &check;      |
