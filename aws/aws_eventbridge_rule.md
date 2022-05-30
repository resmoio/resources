---
description: Amazon Web Services EventBridge Rule
---
aws_eventbridge_rule
--------------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| accountId          | String             | &cross;      |
| arn                | String             | &cross;      |
| description        | String             | &check;      |
| eventBusName       | String             | &check;      |
| eventPattern       | JSON               | &check;      |
| managedBy          | String             | &check;      |
| name               | String             | &cross;      |
| region             | String             | &cross;      |
| roleArn            | String             | &check;      |
| scheduleExpression | String             | &check;      |
| state              | String             | &check;      |
| tags               | Map<String,String> | &check;      |
| targets            | List<RuleTarget>   | &check;      |

#### RuleTarget
| **Name**                    | **Type**                               | **Nullable** |
| --------------------------- | -------------------------------------- | ------------ |
| accountId                   | String                                 | &cross;      |
| arn                         | String                                 | &cross;      |
| batchParameters             | RuleTarget.BatchParameters             | &check;      |
| deadLetterConfig            | RuleTarget.DeadLetterConfig            | &check;      |
| ecsParameters               | RuleTarget.EcsParameters               | &check;      |
| httpParameters              | RuleTarget.HttpParameters              | &check;      |
| id                          | String                                 | &cross;      |
| input                       | String                                 | &check;      |
| inputPath                   | String                                 | &check;      |
| inputTransformer            | RuleTarget.InputTransformer            | &check;      |
| kinesisParameters           | RuleTarget.KinesisParameters           | &check;      |
| redshiftDataParameters      | RuleTarget.RedshiftDataParameters      | &check;      |
| region                      | String                                 | &cross;      |
| retryPolicy                 | RuleTarget.RetryPolicy                 | &check;      |
| roleArn                     | String                                 | &check;      |
| runCommandParameters        | RuleTarget.RunCommandParameters        | &check;      |
| sageMakerPipelineParameters | RuleTarget.SageMakerPipelineParameters | &check;      |
| sqsParameters               | RuleTarget.SqsParameters               | &check;      |

#### RuleTarget.BatchParameters
| **Name**        | **Type**                                        | **Nullable** |
| --------------- | ----------------------------------------------- | ------------ |
| arrayProperties | RuleTarget.BatchParameters.BatchArrayProperties | &check;      |
| jobDefinition   | String                                          | &check;      |
| jobName         | String                                          | &check;      |
| retryStrategy   | RuleTarget.BatchParameters.BatchRetryStrategy   | &check;      |

#### RuleTarget.BatchParameters.BatchArrayProperties
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| size     | Int      | &check;      |

#### RuleTarget.BatchParameters.BatchRetryStrategy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| attempts | Int      | &check;      |

#### RuleTarget.DeadLetterConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &check;      |

#### RuleTarget.EcsParameters
| **Name**                 | **Type**                                                    | **Nullable** |
| ------------------------ | ----------------------------------------------------------- | ------------ |
| capacityProviderStrategy | List<RuleTarget.EcsParameters.CapacityProviderStrategyItem> | &check;      |
| enableECSManagedTags     | Boolean                                                     | &check;      |
| enableExecuteCommand     | Boolean                                                     | &check;      |
| group                    | String                                                      | &check;      |
| launchType               | String                                                      | &check;      |
| networkConfiguration     | RuleTarget.EcsParameters.NetworkConfiguration               | &check;      |
| placementConstraints     | List<RuleTarget.EcsParameters.PlacementConstraint>          | &check;      |
| placementStrategy        | List<RuleTarget.EcsParameters.PlacementStrategy>            | &check;      |
| platformVersion          | String                                                      | &check;      |
| propagateTags            | String                                                      | &check;      |
| referenceId              | String                                                      | &check;      |
| tags                     | Map<String,String>                                          | &check;      |
| taskCount                | Int                                                         | &check;      |
| taskDefinitionArn        | String                                                      | &check;      |

#### RuleTarget.EcsParameters.CapacityProviderStrategyItem
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| base             | Int      | &check;      |
| capacityProvider | String   | &check;      |
| weight           | Int      | &check;      |

#### RuleTarget.EcsParameters.NetworkConfiguration
| **Name**            | **Type**                                                          | **Nullable** |
| ------------------- | ----------------------------------------------------------------- | ------------ |
| awsvpcConfiguration | RuleTarget.EcsParameters.NetworkConfiguration.AwsVpcConfiguration | &check;      |

#### RuleTarget.EcsParameters.NetworkConfiguration.AwsVpcConfiguration
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| assignPublicIp | String       | &check;      |
| securityGroups | List<String> | &check;      |
| subnets        | List<String> | &check;      |

#### RuleTarget.EcsParameters.PlacementConstraint
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| expression | String   | &check;      |
| type       | String   | &check;      |

#### RuleTarget.EcsParameters.PlacementStrategy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| field    | String   | &check;      |
| type     | String   | &check;      |

#### RuleTarget.HttpParameters
| **Name**              | **Type**           | **Nullable** |
| --------------------- | ------------------ | ------------ |
| headerParameters      | Map<String,String> | &check;      |
| pathParameterValues   | List<String>       | &check;      |
| queryStringParameters | Map<String,String> | &check;      |

#### RuleTarget.InputTransformer
| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| inputPathsMap | Map<String,String> | &check;      |
| inputTemplate | String             | &check;      |

#### RuleTarget.KinesisParameters
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| partitionKeyPath | String   | &check;      |

#### RuleTarget.RedshiftDataParameters
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| database         | String   | &check;      |
| dbUser           | String   | &check;      |
| secretManagerArn | String   | &check;      |
| sql              | String   | &check;      |
| statementName    | String   | &check;      |
| withEvent        | Boolean  | &check;      |

#### RuleTarget.RetryPolicy
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| maximumEventAgeInSeconds | Int      | &check;      |
| maximumRetryAttempts     | Int      | &check;      |

#### RuleTarget.RunCommandParameters
| **Name**          | **Type**                                               | **Nullable** |
| ----------------- | ------------------------------------------------------ | ------------ |
| runCommandTargets | List<RuleTarget.RunCommandParameters.RunCommandTarget> | &check;      |

#### RuleTarget.RunCommandParameters.RunCommandTarget
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &check;      |
| values   | List<String> | &check;      |

#### RuleTarget.SageMakerPipelineParameters
| **Name**              | **Type**                                                                | **Nullable** |
| --------------------- | ----------------------------------------------------------------------- | ------------ |
| pipelineParameterList | List<RuleTarget.SageMakerPipelineParameters.SageMakerPipelineParameter> | &check;      |

#### RuleTarget.SageMakerPipelineParameters.SageMakerPipelineParameter
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### RuleTarget.SqsParameters
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| messageGroupId | String   | &check;      |
