---
description: Amazon Web Services AppSync Function
---
aws_appsync_function
--------------------

| **Name**                | **Type**       | **Nullable** |
| ----------------------- | -------------- | ------------ |
| accountId               | String         | &cross;      |
| accountName             | String         | &check;      |
| apiId                   | String         | &cross;      |
| dataSourceName          | String         | &check;      |
| description             | String         | &check;      |
| functionArn             | String         | &check;      |
| functionId              | String         | &cross;      |
| functionVersion         | String         | &check;      |
| maxBatchSize            | Int            | &check;      |
| name                    | String         | &check;      |
| region                  | String         | &cross;      |
| requestMappingTemplate  | String         | &check;      |
| responseMappingTemplate | String         | &check;      |
| runtime                 | AppSyncRuntime | &check;      |
| syncConfig              | SyncConfig     | &check;      |

#### AppSyncRuntime
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| name           | String   | &check;      |
| runtimeVersion | String   | &check;      |

#### LambdaConflictHandlerConfig
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| lambdaConflictHandlerArn | String   | &check;      |

#### SyncConfig
| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| conflictDetection           | String                      | &check;      |
| conflictHandler             | String                      | &check;      |
| lambdaConflictHandlerConfig | LambdaConflictHandlerConfig | &check;      |
