---
description: Amazon Web Services Elastic Beanstalk Environment
---
aws_elasticbeanstalk_environment
--------------------------------

| **Name**                     | **Type**                        | **Nullable** |
| ---------------------------- | ------------------------------- | ------------ |
| abortableOperationInProgress | Boolean                         | &check;      |
| accountId                    | String                          | &cross;      |
| accountName                  | String                          | &check;      |
| applicationName              | String                          | &check;      |
| cname                        | String                          | &check;      |
| dateCreated                  | String                          | &check;      |
| dateUpdated                  | String                          | &check;      |
| description                  | String                          | &check;      |
| endpointURL                  | String                          | &check;      |
| environmentArn               | String                          | &cross;      |
| environmentId                | String                          | &check;      |
| environmentLinks             | List<EnvironmentLink>           | &check;      |
| environmentName              | String                          | &check;      |
| health                       | String                          | &check;      |
| healthStatus                 | String                          | &check;      |
| managedActions               | List<ManagedAction>             | &check;      |
| operationsRole               | String                          | &check;      |
| platformArn                  | String                          | &check;      |
| region                       | String                          | &cross;      |
| resources                    | EnvironmentResourcesDescription | &check;      |
| solutionStackName            | String                          | &check;      |
| status                       | String                          | &check;      |
| templateName                 | String                          | &check;      |
| tier                         | EnvironmentTier                 | &check;      |
| versionLabel                 | String                          | &check;      |

#### EnvironmentLink
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| environmentName | String   | &check;      |
| linkName        | String   | &check;      |

#### EnvironmentResourcesDescription
| **Name**     | **Type**                | **Nullable** |
| ------------ | ----------------------- | ------------ |
| loadBalancer | LoadBalancerDescription | &check;      |

#### EnvironmentTier
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |
| version  | String   | &check;      |

#### Listener
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| port     | Int      | &check;      |
| protocol | String   | &check;      |

#### LoadBalancerDescription
| **Name**         | **Type**       | **Nullable** |
| ---------------- | -------------- | ------------ |
| domain           | String         | &check;      |
| listeners        | List<Listener> | &check;      |
| loadBalancerName | String         | &check;      |

#### ManagedAction
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| actionDescription | String   | &check;      |
| actionId          | String   | &check;      |
| actionType        | String   | &check;      |
| status            | String   | &check;      |
| windowStartTime   | String   | &check;      |
