---
description: Amazon Web Services ECS Task
---
aws_ecs_task
------------

| **Name**              | **Type**                   | **Nullable** |
| --------------------- | -------------------------- | ------------ |
| accountId             | String                     | &cross;      |
| accountName           | String                     | &check;      |
| arn                   | String                     | &cross;      |
| attachments           | List<Attachment>           | &cross;      |
| attributes            | List<Attribute>            | &cross;      |
| capacityProviderName  | String                     | &check;      |
| clusterArn            | String                     | &check;      |
| connectivity          | String                     | &check;      |
| containerInstanceArn  | String                     | &check;      |
| containers            | List<Container>            | &cross;      |
| cpu                   | String                     | &cross;      |
| createdAt             | String                     | &cross;      |
| desiredStatus         | String                     | &cross;      |
| enableExecuteCommand  | Boolean                    | &cross;      |
| ephemeralStorage      | EphemeralStorage           | &check;      |
| executionStoppedAt    | String                     | &check;      |
| healthStatus          | String                     | &cross;      |
| inferenceAccelerators | List<InferenceAccelerator> | &cross;      |
| launchType            | String                     | &cross;      |
| memory                | String                     | &cross;      |
| overrides             | TaskOverride               | &check;      |
| platformFamily        | String                     | &check;      |
| platformVersion       | String                     | &check;      |
| region                | String                     | &cross;      |
| startedAt             | String                     | &check;      |
| startedBy             | String                     | &check;      |
| stopCode              | String                     | &check;      |
| stoppedReason         | String                     | &check;      |
| tags                  | Map<String,String>         | &cross;      |
| taskDefinitionArn     | String                     | &check;      |
| version               | Long                       | &check;      |

#### Attachment
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| details  | Map<String,String> | &check;      |
| id       | String             | &check;      |
| status   | String             | &check;      |
| type     | String             | &check;      |

#### Attribute
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| name       | String   | &check;      |
| targetId   | String   | &check;      |
| targetType | String   | &check;      |
| value      | String   | &check;      |

#### Container
| **Name**          | **Type**                         | **Nullable** |
| ----------------- | -------------------------------- | ------------ |
| containerArn      | String                           | &cross;      |
| cpu               | String                           | &cross;      |
| gpuIds            | List<String>                     | &cross;      |
| healthStatus      | String                           | &check;      |
| image             | String                           | &check;      |
| imageDigest       | String                           | &check;      |
| managedAgents     | List<Container.ManagedAgent>     | &cross;      |
| memory            | String                           | &check;      |
| memoryReservation | String                           | &check;      |
| name              | String                           | &check;      |
| networkBindings   | List<Container.NetworkBinding>   | &cross;      |
| networkInterfaces | List<Container.NetworkInterface> | &cross;      |
| runtimeId         | String                           | &check;      |
| taskArn           | String                           | &check;      |

#### Container.ManagedAgent
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| reason   | String   | &check;      |

#### Container.NetworkBinding
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| bindIP        | String   | &cross;      |
| containerPort | Int      | &cross;      |
| hostPort      | Int      | &cross;      |
| protocol      | String   | &cross;      |

#### Container.NetworkInterface
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| attachmentId       | String   | &check;      |
| ipv6Address        | String   | &check;      |
| privateIpv4Address | String   | &check;      |

#### EphemeralStorage
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| sizeInGiB | Int      | &check;      |

#### InferenceAccelerator
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| deviceName | String   | &cross;      |
| deviceType | String   | &cross;      |

#### TaskOverride
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| cpu      | String   | &check;      |
