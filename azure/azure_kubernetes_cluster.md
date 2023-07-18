---
description: Azure Kubernetes Cluster
---
azure_kubernetes_cluster
------------------------

| **Name**                                        | **Type**                               | **Nullable** |
| ----------------------------------------------- | -------------------------------------- | ------------ |
| aadProfile                                      | AadProfile                             | &check;      |
| addonProfiles                                   | Map<String,ManagedClusterAddonProfile> | &check;      |
| agentPools                                      | List<KubernetesClusterAgentPool>       | &check;      |
| apiAccessProfile                                | ApiAccessProfile                       | &check;      |
| autoScalerProfile                               | AutoScalerProfile                      | &check;      |
| autoUpgradeProfileChannel                       | String                                 | &check;      |
| azurePortalFqdn                                 | String                                 | &check;      |
| disableLocalAccounts                            | Boolean                                | &check;      |
| diskEncryptionSetId                             | String                                 | &check;      |
| dnsPrefix                                       | String                                 | &check;      |
| enablePodSecurityPolicy                         | Boolean                                | &check;      |
| enableRBAC                                      | Boolean                                | &check;      |
| fqdn                                            | String                                 | &check;      |
| fqdnSubdomain                                   | String                                 | &check;      |
| httpProxyConfig                                 | HttpProxyConfig                        | &check;      |
| id                                              | String                                 | &cross;      |
| identity                                        | Identity                               | &check;      |
| linuxRootName                                   | String                                 | &check;      |
| maxAgentPools                                   | Int                                    | &check;      |
| name                                            | String                                 | &cross;      |
| networkProfile                                  | NetworkProfile                         | &check;      |
| nodeResourceGroup                               | String                                 | &check;      |
| podIdentityProfile                              | PodIdentityProfile                     | &check;      |
| powerState                                      | String                                 | &check;      |
| privateEndpointConnections                      | List<PrivateEndpointConnection>        | &check;      |
| privateFqdn                                     | String                                 | &check;      |
| privateLinkResources                            | List<PrivateLinkResource>              | &check;      |
| provisioningState                               | String                                 | &check;      |
| publicNetworkAccess                             | String                                 | &check;      |
| resourceGroupName                               | String                                 | &cross;      |
| securityProfile                                 | SecurityProfile                        | &check;      |
| servicePrincipalClientId                        | String                                 | &check;      |
| servicePrincipalSecret                          | String                                 | &check;      |
| sku                                             | Sku                                    | &check;      |
| subscriptionId                                  | String                                 | &cross;      |
| systemAssignedManagedServiceIdentityPrincipalId | String                                 | &check;      |
| type                                            | String                                 | &cross;      |
| version                                         | String                                 | &check;      |

#### AadProfile
| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| adminGroupObjectIDs | List<String> | &check;      |
| clientAppId         | String       | &check;      |
| enableAzureRbac     | Boolean      | &check;      |
| managed             | Boolean      | &check;      |
| serverAppId         | String       | &check;      |
| serverAppSecret     | String       | &check;      |
| tenantId            | String       | &check;      |

#### ApiAccessProfile
| **Name**                       | **Type**     | **Nullable** |
| ------------------------------ | ------------ | ------------ |
| authorizedIpRanges             | List<String> | &check;      |
| disableRunCommand              | Boolean      | &check;      |
| enablePrivateCluster           | Boolean      | &check;      |
| enablePrivateClusterPublicFqdn | Boolean      | &check;      |
| privateDnsZone                 | String       | &check;      |

#### AutoScalerProfile
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| balanceSimilarNodeGroups      | String   | &check;      |
| expander                      | String   | &check;      |
| maxEmptyBulkDelete            | String   | &check;      |
| maxGracefulTerminationSec     | String   | &check;      |
| maxNodeProvisionTime          | String   | &check;      |
| maxTotalUnreadyPercentage     | String   | &check;      |
| newPodScaleUpDelay            | String   | &check;      |
| okTotalUnreadyCount           | String   | &check;      |
| scaleDownDelayAfterAdd        | String   | &check;      |
| scaleDownDelayAfterDelete     | String   | &check;      |
| scaleDownDelayAfterFailure    | String   | &check;      |
| scaleDownUnneededTime         | String   | &check;      |
| scaleDownUnreadyTime          | String   | &check;      |
| scaleDownUtilizationThreshold | String   | &check;      |
| scanInterval                  | String   | &check;      |
| skipNodesWithLocalStorage     | String   | &check;      |
| skipNodesWithSystemPods       | String   | &check;      |

#### AzureKeyVaultKms
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| enabled               | Boolean  | &check;      |
| keyId                 | String   | &check;      |
| keyVaultNetworkAccess | String   | &check;      |
| keyVaultResourceId    | String   | &check;      |

#### HttpProxyConfig
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| httpProxy  | String       | &check;      |
| httpsProxy | String       | &check;      |
| noProxy    | List<String> | &check;      |
| trustedCa  | String       | &check;      |

#### Identity
| **Name**               | **Type**                         | **Nullable** |
| ---------------------- | -------------------------------- | ------------ |
| principalId            | String                           | &check;      |
| tenantId               | String                           | &check;      |
| type                   | String                           | &check;      |
| userAssignedIdentities | Map<String,UserAssignedIdentity> | &check;      |

#### KubeletConfig
| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| allowedUnsafeSysctls  | List<String> | &check;      |
| containerLogMaxFiles  | Int          | &check;      |
| containerLogMaxSizeMB | Int          | &check;      |
| cpuCfsQuota           | Boolean      | &check;      |
| cpuCfsQuotaPeriod     | String       | &check;      |
| cpuManagerPolicy      | String       | &check;      |
| failSwapOn            | Boolean      | &check;      |
| imageGcHighThreshold  | Int          | &check;      |
| imageGcLowThreshold   | Int          | &check;      |
| podMaxPids            | Int          | &check;      |
| topologyManagerPolicy | String       | &check;      |

#### KubernetesClusterAgentPool
| **Name**                     | **Type**           | **Nullable** |
| ---------------------------- | ------------------ | ------------ |
| availabilityZones            | List<String>       | &check;      |
| count                        | Int                | &check;      |
| creationSourceResourceId     | String             | &check;      |
| enableAutoScaling            | Boolean            | &check;      |
| enableEncryptionAtHost       | Boolean            | &check;      |
| enableFips                   | Boolean            | &check;      |
| enableNodePublicIp           | Boolean            | &check;      |
| enableUltraSsd               | Boolean            | &check;      |
| gpuInstanceProfile           | String             | &check;      |
| isAutoScalingEnabled         | Boolean            | &check;      |
| kubeletConfig                | KubeletConfig      | &check;      |
| kubeletDiskType              | String             | &check;      |
| linuxOSConfig                | LinuxOSConfig      | &check;      |
| maxCount                     | Int                | &check;      |
| maxPods                      | Int                | &check;      |
| maximumPodsPerNode           | Int                | &check;      |
| minCount                     | Int                | &check;      |
| minimumNodeSize              | Int                | &check;      |
| mode                         | String             | &check;      |
| name                         | String             | &check;      |
| networkId                    | String             | &check;      |
| nodeImageVersion             | String             | &check;      |
| nodeLabels                   | Map<String,String> | &check;      |
| nodePublicIpPrefixId         | String             | &check;      |
| nodeSize                     | Int                | &check;      |
| nodeTaints                   | List<String>       | &check;      |
| orchestratorVersion          | String             | &check;      |
| osDiskSizeInGB               | Int                | &check;      |
| osDiskType                   | String             | &check;      |
| osSku                        | String             | &check;      |
| osType                       | String             | &cross;      |
| podSubnetId                  | String             | &check;      |
| powerState                   | String             | &check;      |
| provisioningState            | String             | &cross;      |
| proximityPlacementGroupId    | String             | &check;      |
| scaleDownMode                | String             | &check;      |
| scaleSetEvictionPolicy       | String             | &check;      |
| scaleSetPriority             | String             | &check;      |
| spotMaxPrice                 | Double             | &check;      |
| subnetName                   | String             | &check;      |
| tags                         | Map<String,String> | &check;      |
| type                         | String             | &check;      |
| upgradeMaxSurge              | String             | &check;      |
| virtualMachineEvictionPolicy | String             | &check;      |
| virtualMachineMaximumPrice   | Double             | &check;      |
| virtualMachinePriority       | String             | &check;      |
| vmSize                       | String             | &check;      |
| vnetSubnetId                 | String             | &check;      |
| workloadRuntime              | String             | &check;      |

#### LinuxOSConfig
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| swapFileSizeMB             | Int      | &check;      |
| sysctls                    | JSON     | &check;      |
| transparentHugePageDefrag  | String   | &check;      |
| transparentHugePageEnabled | String   | &check;      |

#### ManagedClusterAddonProfile
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| clientId   | String             | &check;      |
| config     | Map<String,String> | &check;      |
| enabled    | Boolean            | &check;      |
| objectId   | String             | &check;      |
| resourceId | String             | &check;      |

#### NetworkProfile
| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| dnsServiceIP        | String       | &check;      |
| ipFamilies          | List<String> | &check;      |
| loadBalancerProfile | JSON         | &check;      |
| loadBalancerSku     | String       | &check;      |
| natGatewayProfile   | JSON         | &check;      |
| networkDataplane    | String       | &check;      |
| networkMode         | String       | &check;      |
| networkPlugin       | String       | &check;      |
| networkPluginMode   | String       | &check;      |
| networkPolicy       | String       | &check;      |
| outboundType        | String       | &check;      |
| podCidr             | String       | &check;      |
| podCidrs            | List<String> | &check;      |
| serviceCidr         | String       | &check;      |
| serviceCidrs        | List<String> | &check;      |

#### PodIdentity
| **Name**          | **Type**                     | **Nullable** |
| ----------------- | ---------------------------- | ------------ |
| bindingSelector   | String                       | &check;      |
| identity          | UserAssignedIdentity         | &check;      |
| name              | String                       | &check;      |
| namespace         | String                       | &check;      |
| provisioningInfo  | PodIdentityProvisioningError | &check;      |
| provisioningState | String                       | &check;      |

#### PodIdentityException
| **Name**  | **Type**           | **Nullable** |
| --------- | ------------------ | ------------ |
| name      | String             | &check;      |
| namespace | String             | &check;      |
| podLabels | Map<String,String> | &check;      |

#### PodIdentityProfile
| **Name**                       | **Type**                   | **Nullable** |
| ------------------------------ | -------------------------- | ------------ |
| allowNetworkPluginKubenet      | Boolean                    | &check;      |
| enabled                        | Boolean                    | &check;      |
| userAssignedIdentities         | List<PodIdentity>          | &check;      |
| userAssignedIdentityExceptions | List<PodIdentityException> | &check;      |

#### PodIdentityProvisioningError
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| message  | String   | &check;      |
| target   | String   | &check;      |

#### PrivateEndpointConnection
| **Name**                          | **Type**                          | **Nullable** |
| --------------------------------- | --------------------------------- | ------------ |
| id                                | String                            | &cross;      |
| name                              | String                            | &cross;      |
| privateEndpointId                 | String                            | &check;      |
| privateLinkServiceConnectionState | PrivateLinkServiceConnectionState | &check;      |
| provisioningState                 | String                            | &check;      |
| type                              | String                            | &cross;      |

#### PrivateLinkResource
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| groupId              | String       | &check;      |
| requiredDnsZoneNames | List<String> | &check;      |
| requiredMembers      | List<String> | &check;      |

#### PrivateLinkServiceConnectionState
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| actionsRequired | String   | &check;      |
| description     | String   | &check;      |
| status          | String   | &check;      |

#### SecurityProfile
| **Name**         | **Type**                        | **Nullable** |
| ---------------- | ------------------------------- | ------------ |
| azureKeyVaultKms | AzureKeyVaultKms                | &check;      |
| defender         | SecurityProfileDefender         | &check;      |
| imageCleaner     | SecurityProfileImageCleaner     | &check;      |
| workloadIdentity | SecurityProfileWorkloadIdentity | &check;      |

#### SecurityProfileDefender
| **Name**                        | **Type**                                  | **Nullable** |
| ------------------------------- | ----------------------------------------- | ------------ |
| logAnalyticsWorkspaceResourceId | String                                    | &check;      |
| securityMonitoring              | SecurityProfileDefenderSecurityMonitoring | &check;      |

#### SecurityProfileDefenderSecurityMonitoring
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### SecurityProfileImageCleaner
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| enabled       | Boolean  | &check;      |
| intervalHours | Int      | &check;      |

#### SecurityProfileWorkloadIdentity
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### Sku
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| tier     | String   | &check;      |

#### UserAssignedIdentity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| clientId    | String   | &check;      |
| objectId    | String   | &check;      |
| principalId | String   | &check;      |
| resourceId  | String   | &check;      |
