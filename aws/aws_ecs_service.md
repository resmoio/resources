---
description: Amazon Web Services ECS Service
---
aws_ecs_service
---------------

| **Name**                      | **Type**                       | **Nullable** |
| ----------------------------- | ------------------------------ | ------------ |
| accountId                     | String                         | &cross;      |
| arn                           | String                         | &cross;      |
| capacityProviderStrategy      | List<CapacityProviderStrategy> | &check;      |
| clusterArn                    | String                         | &cross;      |
| createdAt                     | String                         | &check;      |
| createdBy                     | String                         | &check;      |
| deploymentConfiguration       | DeploymentConfiguration        | &check;      |
| deploymentController          | DeploymentController           | &check;      |
| deployments                   | List<Deployment>               | &check;      |
| desiredCount                  | Int                            | &check;      |
| enableECSManagedTags          | Boolean                        | &check;      |
| enableExecuteCommand          | Boolean                        | &check;      |
| healthCheckGracePeriodSeconds | Int                            | &check;      |
| launchType                    | String                         | &check;      |
| loadBalancers                 | List<LoadBalancer>             | &check;      |
| name                          | String                         | &check;      |
| networkConfiguration          | NetworkConfiguration           | &check;      |
| placementConstraints          | List<PlacementConstraint>      | &check;      |
| placementStrategy             | List<PlacementStrategy>        | &check;      |
| platformFamily                | String                         | &check;      |
| platformVersion               | String                         | &check;      |
| propagateTasks                | String                         | &check;      |
| region                        | String                         | &cross;      |
| roleArn                       | String                         | &check;      |
| schedulingStrategy            | String                         | &check;      |
| serviceRegistries             | List<ServiceRegistry>          | &check;      |
| taskDefinition                | String                         | &check;      |

#### CapacityProviderStrategy
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| base             | Int      | &check;      |
| capacityProvider | String   | &check;      |
| weight           | Int      | &check;      |

#### Deployment
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| id           | String   | &check;      |
| rolloutState | String   | &check;      |
| status       | String   | &check;      |

#### DeploymentConfiguration
| **Name**                 | **Type**                                         | **Nullable** |
| ------------------------ | ------------------------------------------------ | ------------ |
| deploymentCircuitBreaker | DeploymentConfiguration.DeploymentCircuitBreaker | &check;      |
| maximumPercent           | Int                                              | &check;      |
| minimumHealthyPercent    | Int                                              | &check;      |

#### DeploymentConfiguration.DeploymentCircuitBreaker
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enable   | Boolean  | &check;      |
| rollback | Boolean  | &check;      |

#### DeploymentController
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### LoadBalancer
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| containerName    | String   | &check;      |
| containerPort    | Int      | &check;      |
| loadBalancerName | String   | &check;      |
| targetGroupArn   | String   | &check;      |

#### NetworkConfiguration
| **Name**            | **Type**                                 | **Nullable** |
| ------------------- | ---------------------------------------- | ------------ |
| awsVpcConfiguration | NetworkConfiguration.AwsVpcConfiguration | &check;      |

#### NetworkConfiguration.AwsVpcConfiguration
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| assignPublicIp | String       | &check;      |
| securityGroups | List<String> | &check;      |
| subnets        | List<String> | &check;      |

#### PlacementConstraint
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| expression | String   | &check;      |
| type       | String   | &check;      |

#### PlacementStrategy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| field    | String   | &check;      |
| type     | String   | &check;      |

#### ServiceRegistry
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| containerName | String   | &check;      |
| containerPort | Int      | &check;      |
| port          | Int      | &check;      |
| registryArn   | String   | &check;      |
