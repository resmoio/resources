---
description: Azure Container Group
---
azure_container_group
---------------------

| **Name**                        | **Type**                      | **Nullable** |
| ------------------------------- | ----------------------------- | ------------ |
| containers                      | Map<String,Container>         | &check;      |
| dnsConfig                       | DnsConfiguration              | &check;      |
| encryptionProperties            | EncryptionProperties          | &check;      |
| events                          | List<Event>                   | &check;      |
| externalPorts                   | List<Port>                    | &check;      |
| externalTcpPorts                | List<Int>                     | &check;      |
| externalUdpPorts                | List<Int>                     | &check;      |
| fqdn                            | String                        | &check;      |
| id                              | String                        | &cross;      |
| identity                        | Identity                      | &check;      |
| imageRegistryCredential         | List<ImageRegistryCredential> | &check;      |
| imageRegistryServers            | List<String>                  | &check;      |
| ipAddress                       | String                        | &check;      |
| isIPAddressPrivate              | Boolean                       | &check;      |
| isIPAddressPublic               | Boolean                       | &check;      |
| isManagedServiceIdentityEnabled | Boolean                       | &check;      |
| location                        | String                        | &cross;      |
| logAnalytics                    | LogAnalytics                  | &check;      |
| name                            | String                        | &cross;      |
| osType                          | String                        | &check;      |
| provisioningState               | String                        | &check;      |
| resourceGroupName               | String                        | &cross;      |
| restartPolicy                   | String                        | &check;      |
| sku                             | String                        | &check;      |
| state                           | String                        | &check;      |
| subnetIds                       | List<ContainerGroupSubnetId>  | &check;      |
| subscriptionId                  | String                        | &cross;      |
| tags                            | Map<String,String>            | &check;      |
| type                            | String                        | &cross;      |
| volumes                         | Map<String,Volume>            | &check;      |
| zones                           | List<String>                  | &check;      |

#### AzureFileVolume
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| readOnly           | Boolean  | &check;      |
| shareName          | String   | &check;      |
| storageAccountKey  | String   | &check;      |
| storageAccountName | String   | &check;      |

#### Container
| **Name**             | **Type**                        | **Nullable** |
| -------------------- | ------------------------------- | ------------ |
| command              | List<String>                    | &check;      |
| environmentVariables | List<EnvironmentVariable>       | &check;      |
| image                | String                          | &check;      |
| instanceView         | ContainerPropertiesInstanceView | &check;      |
| livenessProbe        | ContainerProbe                  | &check;      |
| name                 | String                          | &check;      |
| ports                | List<ContainerPort>             | &check;      |
| readinessProbe       | ContainerProbe                  | &check;      |
| resources            | ResourceRequirements            | &check;      |
| volumeMounts         | List<VolumeMount>               | &check;      |

#### ContainerGroupSubnetId
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### ContainerHttpGet
| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| httpHeaders | Map<String,String> | &check;      |
| path        | String             | &check;      |
| port        | Int                | &check;      |
| scheme      | String             | &check;      |

#### ContainerPort
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| port     | Int      | &check;      |
| protocol | String   | &check;      |

#### ContainerProbe
| **Name**            | **Type**         | **Nullable** |
| ------------------- | ---------------- | ------------ |
| command             | List<String>     | &check;      |
| failureThreshold    | Int              | &check;      |
| httpGet             | ContainerHttpGet | &check;      |
| initialDelaySeconds | Int              | &check;      |
| periodSeconds       | Int              | &check;      |
| successThreshold    | Int              | &check;      |
| timeoutSeconds      | Int              | &check;      |

#### ContainerPropertiesInstanceView
| **Name**      | **Type**       | **Nullable** |
| ------------- | -------------- | ------------ |
| currentState  | ContainerState | &check;      |
| events        | List<Event>    | &check;      |
| previousState | ContainerState | &check;      |
| restartCount  | Int            | &check;      |

#### ContainerState
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| detailStatus | String   | &check;      |
| exitCode     | Int      | &check;      |
| finishTime   | String   | &check;      |
| startTime    | String   | &check;      |
| state        | String   | &check;      |

#### DnsConfiguration
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| nameServers   | List<String> | &check;      |
| options       | String       | &check;      |
| searchDomains | String       | &check;      |

#### EncryptionProperties
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| keyName      | String   | &check;      |
| keyVersion   | String   | &check;      |
| vaultBaseUrl | String   | &check;      |

#### EnvironmentVariable
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| name        | String   | &check;      |
| secureValue | String   | &check;      |
| value       | String   | &check;      |

#### Event
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| count          | Int      | &check;      |
| firstTimestamp | String   | &check;      |
| lastTimestamp  | String   | &check;      |
| message        | String   | &check;      |
| name           | String   | &check;      |
| type           | String   | &check;      |

#### GitRepoVolume
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| directory  | String   | &check;      |
| repository | String   | &check;      |
| revision   | String   | &check;      |

#### Identity
| **Name**               | **Type**                         | **Nullable** |
| ---------------------- | -------------------------------- | ------------ |
| principalId            | String                           | &check;      |
| tenantId               | String                           | &check;      |
| type                   | String                           | &check;      |
| userAssignedIdentities | Map<String,UserAssignedIdentity> | &check;      |

#### ImageRegistryCredential
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| identity    | String   | &check;      |
| identityUrl | String   | &check;      |
| password    | String   | &check;      |
| server      | String   | &check;      |
| username    | String   | &check;      |

#### InitContainerDefinition
| **Name**             | **Type**                        | **Nullable** |
| -------------------- | ------------------------------- | ------------ |
| command              | List<String>                    | &check;      |
| environmentVariables | List<EnvironmentVariable>       | &check;      |
| image                | String                          | &check;      |
| instanceView         | ContainerPropertiesInstanceView | &check;      |
| volumeMounts         | List<VolumeMount>               | &check;      |

#### LogAnalytics
| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| logType             | String             | &check;      |
| metadata            | Map<String,String> | &check;      |
| workspaceId         | String             | &check;      |
| workspaceKey        | String             | &check;      |
| workspaceResourceId | String             | &check;      |

#### Port
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| port     | Int      | &check;      |
| protocol | String   | &check;      |

#### Resource
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| cpu        | Double   | &check;      |
| gpuCount   | Int      | &check;      |
| gpuSku     | String   | &check;      |
| memoryInGB | Double   | &check;      |

#### ResourceRequirements
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| limits   | Resource | &check;      |
| requests | Resource | &check;      |

#### UserAssignedIdentity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| clientId    | String   | &check;      |
| principalId | String   | &check;      |

#### Volume
| **Name**  | **Type**           | **Nullable** |
| --------- | ------------------ | ------------ |
| azureFile | AzureFileVolume    | &check;      |
| emptyDir  | String             | &check;      |
| gitRepo   | GitRepoVolume      | &check;      |
| name      | String             | &check;      |
| secret    | Map<String,String> | &check;      |

#### VolumeMount
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| mountPath | String   | &check;      |
| name      | String   | &check;      |
| readOnly  | Boolean  | &check;      |
