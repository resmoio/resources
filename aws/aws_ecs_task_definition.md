---
description: Amazon Web Services ECS Task Definition
---
aws_ecs_task_definition
-----------------------

| **Name**              | **Type**                   | **Nullable** |
| --------------------- | -------------------------- | ------------ |
| accountId             | String                     | &cross;      |
| arn                   | String                     | &cross;      |
| compatibilities       | List<String>               | &check;      |
| containerDefinitions  | List<ContainerDefinition>  | &check;      |
| cpu                   | String                     | &check;      |
| deregisteredAt        | String                     | &check;      |
| ephemeralStorage      | EphemeralStorage           | &check;      |
| executionRoleArn      | String                     | &check;      |
| family                | String                     | &check;      |
| inferenceAccelerators | List<InferenceAccelerator> | &check;      |
| ipcMode               | String                     | &check;      |
| memory                | String                     | &check;      |
| networkMode           | String                     | &check;      |
| pidMode               | String                     | &check;      |
| placementConstraints  | List<PlacementConstraint>  | &check;      |
| proxyConfiguration    | ProxyConfiguration         | &check;      |
| region                | String                     | &check;      |
| registeredAt          | String                     | &check;      |
| registeredBy          | String                     | &check;      |
| requiresAttributes    | List<RequireAttribute>     | &check;      |
| revision              | Int                        | &check;      |
| taskDefinitionArn     | String                     | &check;      |
| taskRoleArn           | String                     | &check;      |
| volumes               | List<Volume>               | &check;      |

#### ContainerDefinition
| **Name**               | **Type**                                      | **Nullable** |
| ---------------------- | --------------------------------------------- | ------------ |
| command                | List<String>                                  | &check;      |
| cpu                    | Int                                           | &check;      |
| dependsOn              | List<ContainerDefinition.ContainerDependency> | &check;      |
| disableNetworking      | Boolean                                       | &check;      |
| dnsSearchDomains       | List<String>                                  | &check;      |
| dnsServers             | List<String>                                  | &check;      |
| dockerLabels           | Map<String,String>                            | &check;      |
| dockerSecurityOptions  | List<String>                                  | &check;      |
| entryPoint             | List<String>                                  | &check;      |
| environment            | Map<String,String>                            | &check;      |
| environmentFiles       | List<ContainerDefinition.EnvironmentFile>     | &check;      |
| essential              | Boolean                                       | &check;      |
| extraHosts             | List<ContainerDefinition.HostEntry>           | &check;      |
| firelensConfiguration  | ContainerDefinition.FirelensConfiguration     | &check;      |
| healthCheck            | ContainerDefinition.HealthCheck               | &check;      |
| image                  | String                                        | &check;      |
| interactive            | Boolean                                       | &check;      |
| links                  | List<String>                                  | &check;      |
| linuxParameters        | ContainerDefinition.LinuxParameters           | &check;      |
| logConfiguration       | ContainerDefinition.LogConfiguration          | &check;      |
| memory                 | Int                                           | &check;      |
| memoryReservation      | Int                                           | &check;      |
| mountPoints            | List<ContainerDefinition.MountPoint>          | &check;      |
| name                   | String                                        | &check;      |
| portMappings           | List<ContainerDefinition.PortMapping>         | &check;      |
| privileged             | Boolean                                       | &check;      |
| pseudoTerminal         | Boolean                                       | &check;      |
| readonlyRootFilesystem | Boolean                                       | &check;      |
| repositoryCredentials  | ContainerDefinition.RepositoryCredentials     | &check;      |
| resourceRequirements   | List<ContainerDefinition.ResourceRequirement> | &check;      |
| secrets                | List<ContainerDefinition.Secret>              | &check;      |
| startTimeout           | Int                                           | &check;      |
| stopTimeout            | Int                                           | &check;      |
| systemControls         | List<ContainerDefinition.SystemControl>       | &check;      |
| ulimits                | List<ContainerDefinition.Ulimit>              | &check;      |
| user                   | String                                        | &check;      |
| volumesFrom            | List<ContainerDefinition.VolumeFrom>          | &check;      |
| workingDirectory       | String                                        | &check;      |

#### ContainerDefinition.ContainerDependency
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| condition     | String   | &check;      |
| containerName | String   | &check;      |

#### ContainerDefinition.EnvironmentFile
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| value    | String   | &check;      |

#### ContainerDefinition.FirelensConfiguration
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| options  | Map<String,String> | &check;      |
| type     | String             | &check;      |

#### ContainerDefinition.HealthCheck
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| command     | List<String> | &check;      |
| interval    | Int          | &check;      |
| retries     | Int          | &check;      |
| startPeriod | Int          | &check;      |
| timeout     | Int          | &check;      |

#### ContainerDefinition.HostEntry
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| hostname  | String   | &check;      |
| ipAddress | String   | &check;      |

#### ContainerDefinition.LinuxParameters
| **Name**           | **Type**                                         | **Nullable** |
| ------------------ | ------------------------------------------------ | ------------ |
| capabilities       | ContainerDefinition.LinuxParameters.Capabilities | &check;      |
| initProcessEnabled | Boolean                                          | &check;      |
| maxSwap            | Int                                              | &check;      |
| sharedMemorySize   | Int                                              | &check;      |
| tmpfs              | List<ContainerDefinition.LinuxParameters.Tmpfs>  | &check;      |

#### ContainerDefinition.LinuxParameters.Capabilities
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| add      | List<String> | &check;      |
| drop     | List<String> | &check;      |

#### ContainerDefinition.LinuxParameters.Tmpfs
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| containerPath | String       | &check;      |
| mountOptions  | List<String> | &check;      |
| size          | Int          | &check;      |

#### ContainerDefinition.LogConfiguration
| **Name**      | **Type**                                                 | **Nullable** |
| ------------- | -------------------------------------------------------- | ------------ |
| logDriver     | String                                                   | &check;      |
| options       | Map<String,String>                                       | &check;      |
| secretOptions | List<ContainerDefinition.LogConfiguration.SecretOptions> | &check;      |

#### ContainerDefinition.LogConfiguration.SecretOptions
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| name      | String   | &check;      |
| valueFrom | String   | &check;      |

#### ContainerDefinition.MountPoint
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| containerPath | String   | &check;      |
| readOnly      | Boolean  | &check;      |
| sourceVolume  | String   | &check;      |

#### ContainerDefinition.PortMapping
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| containerPort | Int      | &check;      |
| hostPort      | Int      | &check;      |
| protocol      | String   | &check;      |

#### ContainerDefinition.RepositoryCredentials
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| credentialsParameter | String   | &check;      |

#### ContainerDefinition.ResourceRequirement
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| value    | String   | &check;      |

#### ContainerDefinition.Secret
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| name      | String   | &check;      |
| valueFrom | String   | &check;      |

#### ContainerDefinition.SystemControl
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| namespace | String   | &check;      |
| value     | String   | &check;      |

#### ContainerDefinition.Ulimit
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| hardLimit | Int      | &check;      |
| name      | String   | &check;      |
| softLimit | Int      | &check;      |

#### ContainerDefinition.VolumeFrom
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| readOnly        | Boolean  | &check;      |
| sourceContainer | String   | &check;      |

#### EphemeralStorage
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| sizeInGiB | Int      | &check;      |

#### InferenceAccelerator
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### PlacementConstraint
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| expression | String   | &check;      |
| type       | String   | &check;      |

#### ProxyConfiguration
| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| containerName | String             | &check;      |
| properties    | Map<String,String> | &check;      |
| type          | String             | &check;      |

#### RequireAttribute
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| name       | String   | &check;      |
| targetId   | String   | &check;      |
| targetType | String   | &check;      |
| value      | String   | &check;      |

#### Volume
| **Name**                  | **Type**                         | **Nullable** |
| ------------------------- | -------------------------------- | ------------ |
| dockerVolumeConfiguration | Volume.DockerVolumeConfiguration | &check;      |
| efsVolumeConfiguration    | Volume.EfsVolumeConfiguration    | &check;      |

#### Volume.DockerVolumeConfiguration
| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| autoprovision | Boolean            | &check;      |
| driver        | String             | &check;      |
| driverOpts    | Map<String,String> | &check;      |
| labels        | Map<String,String> | &check;      |
| scope         | String             | &check;      |

#### Volume.EfsVolumeConfiguration
| **Name**                  | **Type**                                          | **Nullable** |
| ------------------------- | ------------------------------------------------- | ------------ |
| authorizationConfig       | Volume.EfsVolumeConfiguration.AuthorizationConfig | &check;      |
| fileSystemId              | String                                            | &check;      |
| rootDirectory             | String                                            | &check;      |
| transitEncryptionAsString | String                                            | &check;      |
| transitEncryptionPort     | Int                                               | &check;      |

#### Volume.EfsVolumeConfiguration.AuthorizationConfig
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| accessPointId | String   | &check;      |
| iam           | String   | &check;      |
