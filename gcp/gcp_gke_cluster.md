---
description: Google Cloud Platform GKE Cluster
---
gcp_gke_cluster
---------------

| **Name**                       | **Type**                       | **Nullable** |
| ------------------------------ | ------------------------------ | ------------ |
| addonsConfig                   | AddonsConfig                   | &check;      |
| authenticatorGroupsConfig      | AuthenticatorGroupsConfig      | &check;      |
| autopilot                      | Autopilot                      | &check;      |
| autoscaling                    | ClusterAutoscaling             | &check;      |
| binaryAuthorization            | BinaryAuthorization            | &check;      |
| clusterIpv4Cidr                | String                         | &check;      |
| conditions                     | List<StatusCondition>          | &check;      |
| confidentialNodes              | ConfidentialNodes              | &check;      |
| createTime                     | String                         | &check;      |
| currentMasterVersion           | String                         | &check;      |
| currentNodeCount               | Int                            | &check;      |
| currentNodeVersion             | String                         | &check;      |
| databaseEncryption             | DatabaseEncryption             | &check;      |
| defaultMaxPodsConstraint       | MaxPodsConstraint              | &check;      |
| description                    | String                         | &check;      |
| enableKubernetesAlpha          | Boolean                        | &check;      |
| enableTpu                      | String                         | &check;      |
| endpoint                       | String                         | &check;      |
| expireTime                     | String                         | &check;      |
| initialClusterVersion          | String                         | &check;      |
| initialNodeCount               | Int                            | &check;      |
| instanceGroupUrls              | List<String>                   | &check;      |
| ipAllocationPolicy             | IPAllocationPolicy             | &check;      |
| legacyAbac                     | LegacyAbac                     | &check;      |
| location                       | String                         | &check;      |
| locations                      | List<String>                   | &check;      |
| loggingConfig                  | LoggingConfig                  | &check;      |
| loggingService                 | String                         | &check;      |
| maintenancePolicy              | MaintenancePolicy              | &check;      |
| masterAuth                     | MasterAuth                     | &check;      |
| masterAuthorizedNetworksConfig | MasterAuthorizedNetworksConfig | &check;      |
| meshCertificates               | MeshCertificates               | &check;      |
| monitoringConfig               | MonitoringConfig               | &check;      |
| monitoringService              | String                         | &check;      |
| name                           | String                         | &cross;      |
| network                        | String                         | &check;      |
| networkConfig                  | NetworkConfig                  | &check;      |
| networkPolicy                  | NetworkPolicy                  | &check;      |
| nodeConfig                     | NodeConfig                     | &check;      |
| nodeIpv4CidrSize               | Int                            | &check;      |
| nodePoolDefaults               | NodePoolDefaults               | &check;      |
| nodePools                      | List<NodePool>                 | &check;      |
| notificationConfig             | NotificationConfig             | &check;      |
| privateClusterConfig           | PrivateClusterConfig           | &check;      |
| project                        | String                         | &cross;      |
| releaseChannel                 | ReleaseChannel                 | &check;      |
| resourceLabels                 | Map<String,String>             | &check;      |
| resourceUsageExportConfig      | ResourceUsageExportConfig      | &check;      |
| servicesIpv4Cidr               | String                         | &check;      |
| shieldedNodes                  | ShieldedNodes                  | &check;      |
| status                         | String                         | &check;      |
| statusMessage                  | String                         | &check;      |
| subnetwork                     | String                         | &check;      |
| tpuIpv4CidrBlock               | String                         | &check;      |
| verticalPodAutoscaling         | VerticalPodAutoscaling         | &check;      |
| workloadIdentityConfig         | WorkloadIdentityConfig         | &check;      |
| zone                           | String                         | &check;      |

#### AddonsConfig
| **Name**                         | **Type**                                      | **Nullable** |
| -------------------------------- | --------------------------------------------- | ------------ |
| cloudRunConfig                   | AddonsConfig.CloudRunConfig                   | &check;      |
| configConnectorConfig            | AddonsConfig.ConfigConnectorConfig            | &check;      |
| dnsCacheConfig                   | AddonsConfig.DnsCacheConfig                   | &check;      |
| gcePersistentDiskCsiDriverConfig | AddonsConfig.GcePersistentDiskCsiDriverConfig | &check;      |
| gcpFilestoreCsiDriverConfig      | AddonsConfig.GcpFilestoreCsiDriverConfig      | &check;      |
| horizontalPodAutoscaling         | AddonsConfig.HorizontalPodAutoscaling         | &check;      |
| httpLoadBalancing                | AddonsConfig.HttpLoadBalancing                | &check;      |
| kubernetesDashboard              | AddonsConfig.KubernetesDashboard              | &check;      |
| networkPolicyConfig              | AddonsConfig.NetworkPolicyConfig              | &check;      |

#### AddonsConfig.CloudRunConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| disabled         | Boolean  | &check;      |
| loadBalancerType | String   | &check;      |

#### AddonsConfig.ConfigConnectorConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AddonsConfig.DnsCacheConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AddonsConfig.GcePersistentDiskCsiDriverConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AddonsConfig.GcpFilestoreCsiDriverConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AddonsConfig.HorizontalPodAutoscaling
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AddonsConfig.HttpLoadBalancing
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AddonsConfig.KubernetesDashboard
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AddonsConfig.NetworkPolicyConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### AuthenticatorGroupsConfig
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| enabled       | Boolean  | &check;      |
| securityGroup | String   | &check;      |

#### Autopilot
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### BinaryAuthorization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### CidrBlock
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| cidrBlock   | String   | &check;      |
| displayName | String   | &check;      |

#### ClusterAutoscaling
| **Name**                         | **Type**                                            | **Nullable** |
| -------------------------------- | --------------------------------------------------- | ------------ |
| autoprovisioningLocations        | List<String>                                        | &check;      |
| autoprovisioningNodePoolDefaults | ClusterAutoscaling.AutoprovisioningNodePoolDefaults | &check;      |
| autoscalingProfile               | String                                              | &check;      |
| enableNodeAutoprovisioning       | Boolean                                             | &check;      |
| resourceLimits                   | ClusterAutoscaling.ResourceLimit                    | &check;      |

#### ClusterAutoscaling.AutoprovisioningNodePoolDefaults
| **Name**               | **Type**               | **Nullable** |
| ---------------------- | ---------------------- | ------------ |
| bootDiskKmsKey         | String                 | &check;      |
| diskSizeGb             | Int                    | &check;      |
| diskType               | String                 | &check;      |
| imageType              | String                 | &check;      |
| management             | NodeManagement         | &check;      |
| minCpuPlatform         | String                 | &check;      |
| oauthScopes            | List<String>           | &check;      |
| serviceAccount         | String                 | &check;      |
| shieldedInstanceConfig | ShieldedInstanceConfig | &check;      |
| upgradeSettings        | UpgradeSettings        | &check;      |

#### ClusterAutoscaling.ResourceLimit
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| maximum      | String   | &check;      |
| minimum      | String   | &check;      |
| resourceType | String   | &check;      |

#### ConfidentialNodes
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### DatabaseEncryption
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| keyName  | String   | &check;      |
| state    | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### GcfsConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### IPAllocationPolicy
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| clusterIpv4Cidr            | String   | &check;      |
| clusterIpv4CidrBlock       | String   | &check;      |
| clusterSecondaryRangeName  | String   | &check;      |
| createSubnetwork           | Boolean  | &check;      |
| nodeIpv4Cidr               | String   | &check;      |
| nodeIpv4CidrBlock          | String   | &check;      |
| servicesIpv4Cidr           | String   | &check;      |
| servicesIpv4CidrBlock      | String   | &check;      |
| servicesSecondaryRangeName | String   | &check;      |
| subnetworkName             | String   | &check;      |
| tpuIpv4CidrBlock           | String   | &check;      |
| useIpAliases               | Boolean  | &check;      |
| useRoutes                  | Boolean  | &check;      |

#### LegacyAbac
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### LoggingConfig
| **Name**        | **Type**                             | **Nullable** |
| --------------- | ------------------------------------ | ------------ |
| componentConfig | LoggingConfig.LoggingComponentConfig | &check;      |

#### LoggingConfig.LoggingComponentConfig
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| enableComponents | List<String> | &cross;      |

#### MaintenancePolicy
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| resourceVersion | String   | &check;      |
| window          | JSON     | &check;      |

#### MasterAuth
| **Name**                | **Type**                           | **Nullable** |
| ----------------------- | ---------------------------------- | ------------ |
| clientCertificate       | String                             | &check;      |
| clientCertificateConfig | MasterAuth.ClientCertificateConfig | &check;      |
| clientKey               | String                             | &check;      |
| clusterCaCertificate    | String                             | &check;      |

#### MasterAuth.ClientCertificateConfig
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| issueClientCertificate | Boolean  | &check;      |

#### MasterAuthorizedNetworksConfig
| **Name**   | **Type**  | **Nullable** |
| ---------- | --------- | ------------ |
| cidrBlocks | CidrBlock | &check;      |
| enabled    | Boolean   | &check;      |

#### MaxPodsConstraint
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| maxPodsPerNode | String   | &check;      |

#### MeshCertificates
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| enableCertificates | Boolean  | &check;      |

#### MonitoringConfig
| **Name**        | **Type**                                   | **Nullable** |
| --------------- | ------------------------------------------ | ------------ |
| componentConfig | MonitoringConfig.MonitoringComponentConfig | &check;      |

#### MonitoringConfig.MonitoringComponentConfig
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| enableComponents | List<String> | &check;      |

#### NetworkConfig
| **Name**                  | **Type**                               | **Nullable** |
| ------------------------- | -------------------------------------- | ------------ |
| datapathProvider          | String                                 | &check;      |
| defaultSnatStatus         | NetworkConfig.DefaultSnatStatus        | &check;      |
| dnsConfig                 | NetworkConfig.DNSConfig                | &check;      |
| enableIntraNodeVisibility | Boolean                                | &check;      |
| enableL4ilbSubsetting     | Boolean                                | &check;      |
| network                   | String                                 | &check;      |
| privateIpv6GoogleAccess   | String                                 | &check;      |
| serviceExternalIpsConfig  | NetworkConfig.ServiceExternalIPsConfig | &check;      |
| subnetwork                | String                                 | &check;      |

#### NetworkConfig.DNSConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| clusterDns       | String   | &check;      |
| clusterDnsDomain | String   | &check;      |
| clusterDnsScope  | String   | &check;      |

#### NetworkConfig.DefaultSnatStatus
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| disabled | Boolean  | &check;      |

#### NetworkConfig.ServiceExternalIPsConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### NetworkPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |
| provider | String   | &check;      |

#### NodeConfig
| **Name**                | **Type**                           | **Nullable** |
| ----------------------- | ---------------------------------- | ------------ |
| accelerators            | List<NodeConfig.AcceleratorConfig> | &check;      |
| advancedMachineFeatures | NodeConfig.AdvancedMachineFeatures | &check;      |
| bootDiskKmsKey          | String                             | &check;      |
| diskSizeGb              | Int                                | &check;      |
| diskType                | String                             | &check;      |
| gcfsConfig              | GcfsConfig                         | &check;      |
| gvnic                   | NodeConfig.VirtualNIC              | &check;      |
| imageType               | String                             | &check;      |
| kubeletConfig           | NodeConfig.NodeKubeletConfig       | &check;      |
| labels                  | Map<String,String>                 | &check;      |
| linuxNodeConfig         | NodeConfig.LinuxNodeConfig         | &check;      |
| localSsdCount           | Int                                | &check;      |
| machineType             | String                             | &check;      |
| metadata                | Map<String,String>                 | &check;      |
| minCpuPlatform          | String                             | &check;      |
| nodeGroup               | String                             | &check;      |
| oauthScopes             | List<String>                       | &check;      |
| preemptible             | Boolean                            | &check;      |
| reservationAffinity     | NodeConfig.ReservationAffinity     | &check;      |
| sandboxConfig           | NodeConfig.SandboxConfig           | &check;      |
| serviceAccount          | String                             | &check;      |
| shieldedInstanceConfig  | ShieldedInstanceConfig             | &check;      |
| tags                    | List<String>                       | &check;      |
| taints                  | List<NodeConfig.NodeTaint>         | &check;      |
| workloadMetadataConfig  | NodeConfig.WorkloadMetadataConfig  | &check;      |

#### NodeConfig.AcceleratorConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| acceleratorCount | String   | &check;      |
| acceleratorType  | String   | &check;      |
| gpuPartitionSize | String   | &check;      |

#### NodeConfig.AdvancedMachineFeatures
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| threadsPerCore | String   | &check;      |

#### NodeConfig.LinuxNodeConfig
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| sysctls  | Map<String,String> | &check;      |

#### NodeConfig.NodeKubeletConfig
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| cpuCfsQuota       | Boolean  | &check;      |
| cpuCfsQuotaPeriod | String   | &check;      |
| cpuManagerPolicy  | String   | &check;      |

#### NodeConfig.NodeTaint
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| effect   | String   | &check;      |
| key      | String   | &check;      |
| value    | String   | &check;      |

#### NodeConfig.ReservationAffinity
| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| consumeReservationType | String       | &check;      |
| key                    | String       | &check;      |
| values                 | List<String> | &check;      |

#### NodeConfig.SandboxConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### NodeConfig.VirtualNIC
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### NodeConfig.WorkloadMetadataConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| mode     | String   | &check;      |

#### NodeManagement
| **Name**       | **Type**                          | **Nullable** |
| -------------- | --------------------------------- | ------------ |
| autoRepair     | Boolean                           | &check;      |
| autoUpgrade    | Boolean                           | &check;      |
| upgradeOptions | NodeManagement.AutoUpgradeOptions | &check;      |

#### NodeManagement.AutoUpgradeOptions
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| autoUpgradeStartTime | String   | &check;      |
| description          | String   | &check;      |

#### NodePool
| **Name**          | **Type**                     | **Nullable** |
| ----------------- | ---------------------------- | ------------ |
| autoscaling       | NodePool.NodePoolAutoscaling | &check;      |
| conditions        | List<StatusCondition>        | &check;      |
| config            | NodeConfig                   | &check;      |
| initialNodeCount  | Int                          | &check;      |
| instanceGroupUrls | List<String>                 | &check;      |
| locations         | List<String>                 | &check;      |
| management        | NodeManagement               | &check;      |
| maxPodsConstraint | NodePool.MaxPodsConstraint   | &check;      |
| name              | String                       | &check;      |
| networkConfig     | NodePool.NodeNetworkConfig   | &check;      |
| podIpv4CidrSize   | Int                          | &check;      |
| status            | String                       | &check;      |
| statusMessage     | String                       | &check;      |
| upgradeSettings   | UpgradeSettings              | &check;      |
| version           | String                       | &check;      |

#### NodePool.MaxPodsConstraint
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| maxPodsPerNode | String   | &check;      |

#### NodePool.NodeNetworkConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| createPodRange   | Boolean  | &check;      |
| podIpv4CidrBlock | String   | &check;      |
| podRange         | String   | &check;      |

#### NodePool.NodePoolAutoscaling
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| autoprovisioned | Boolean  | &check;      |
| enabled         | Boolean  | &check;      |
| maxNodeCount    | Int      | &check;      |
| minNodeCount    | Int      | &check;      |

#### NodePoolDefaults
| **Name**           | **Type**                            | **Nullable** |
| ------------------ | ----------------------------------- | ------------ |
| nodeConfigDefaults | NodePoolDefaults.NodeConfigDefaults | &check;      |

#### NodePoolDefaults.NodeConfigDefaults
| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| gcfsConfig | GcfsConfig | &check;      |

#### NotificationConfig
| **Name** | **Type**                  | **Nullable** |
| -------- | ------------------------- | ------------ |
| pubsub   | NotificationConfig.PubSub | &check;      |

#### NotificationConfig.PubSub
| **Name** | **Type**                         | **Nullable** |
| -------- | -------------------------------- | ------------ |
| enabled  | Boolean                          | &check;      |
| filter   | NotificationConfig.PubSub.Filter | &check;      |
| topic    | String                           | &check;      |

#### NotificationConfig.PubSub.Filter
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| eventType | List<String> | &check;      |

#### PrivateClusterConfig
| **Name**                 | **Type**                                                    | **Nullable** |
| ------------------------ | ----------------------------------------------------------- | ------------ |
| enablePrivateEndpoint    | Boolean                                                     | &check;      |
| enablePrivateNodes       | Boolean                                                     | &check;      |
| masterGlobalAccessConfig | PrivateClusterConfig.PrivateClusterMasterGlobalAccessConfig | &check;      |
| masterIpv4CidrBlock      | String                                                      | &check;      |
| peeringName              | String                                                      | &check;      |
| privateEndpoint          | String                                                      | &check;      |
| publicEndpoint           | String                                                      | &check;      |

#### PrivateClusterConfig.PrivateClusterMasterGlobalAccessConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### ReleaseChannel
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| channel  | String   | &check;      |

#### ResourceUsageExportConfig
| **Name**                    | **Type**                                            | **Nullable** |
| --------------------------- | --------------------------------------------------- | ------------ |
| bigqueryDestination         | ResourceUsageExportConfig.BigQueryDestination       | &check;      |
| consumptionMeteringConfig   | ResourceUsageExportConfig.ConsumptionMeteringConfig | &check;      |
| enableNetworkEgressMetering | Boolean                                             | &check;      |

#### ResourceUsageExportConfig.BigQueryDestination
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| datasetId | String   | &check;      |

#### ResourceUsageExportConfig.ConsumptionMeteringConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### ShieldedInstanceConfig
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| enableIntegrityMonitoring | Boolean  | &check;      |
| enableSecureBoot          | Boolean  | &check;      |

#### ShieldedNodes
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### StatusCondition
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| canonicalCode | String   | &check;      |
| code          | String   | &check;      |
| message       | String   | &check;      |

#### UpgradeSettings
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| maxSurge       | Int      | &check;      |
| maxUnavailable | Int      | &check;      |

#### VerticalPodAutoscaling
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### WorkloadIdentityConfig
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| workloadPool | String   | &check;      |
