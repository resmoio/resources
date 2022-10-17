---
description: Qualys Host Asset
---
qualys_host_asset
-----------------

| **Name**                   | **Type**                 | **Nullable** |
| -------------------------- | ------------------------ | ------------ |
| account                    | List<HostAssetAccount>   | &check;      |
| address                    | String                   | &check;      |
| agentInfo                  | AgentInfo                | &check;      |
| biosDescription            | String                   | &check;      |
| cloudProvider              | String                   | &check;      |
| created                    | String                   | &check;      |
| dnsHostName                | String                   | &check;      |
| dockerInfo                 | DockerInfo               | &check;      |
| domain                     | String                   | &check;      |
| fqdn                       | String                   | &check;      |
| id                         | String                   | &cross;      |
| informationGatheredUpdated | String                   | &check;      |
| isDockerHost               | Boolean                  | &check;      |
| lastComplianceScan         | String                   | &check;      |
| lastLoggedOnUser           | String                   | &check;      |
| lastSystemBoot             | String                   | &check;      |
| lastVulnScan               | String                   | &check;      |
| manufacturer               | String                   | &check;      |
| model                      | String                   | &check;      |
| modified                   | String                   | &check;      |
| name                       | String                   | &check;      |
| netbiosName                | String                   | &check;      |
| netbiosNetworkId           | Long                     | &check;      |
| networkGuid                | String                   | &check;      |
| networkInterface           | List<HostAssetInterface> | &check;      |
| openPort                   | List<HostAssetOpenPort>  | &check;      |
| os                         | String                   | &check;      |
| processor                  | List<HostAssetProcessor> | &check;      |
| qwebHostId                 | String                   | &check;      |
| software                   | List<HostAssetSoftware>  | &check;      |
| sourceInfo                 | SourceInfo               | &check;      |
| tags                       | List<Tag>                | &check;      |
| timezone                   | String                   | &check;      |
| totalMemory                | Long                     | &check;      |
| trackingMethod             | String                   | &check;      |
| type                       | String                   | &check;      |
| volume                     | List<HostAssetVolume>    | &check;      |
| vuln                       | List<HostAssetVuln>      | &check;      |
| vulnsUpdated               | String                   | &check;      |

#### AgentInfo
| **Name**            | **Type**                     | **Nullable** |
| ------------------- | ---------------------------- | ------------ |
| activatedModule     | String                       | &check;      |
| activationKey       | AgentInfo.ActivationKey      | &check;      |
| agentConfiguration  | AgentInfo.AgentConfiguration | &check;      |
| agentId             | String                       | &check;      |
| agentVersion        | String                       | &check;      |
| chirpStatus         | String                       | &check;      |
| connectedFrom       | String                       | &check;      |
| lastCheckedIn       | String                       | &check;      |
| localIpv4           | String                       | &check;      |
| localIpv6           | String                       | &check;      |
| location            | String                       | &check;      |
| locationGeoLatitude | String                       | &check;      |
| manifestVersion     | AgentInfo.ManifestVersion    | &check;      |
| platform            | String                       | &check;      |
| status              | String                       | &check;      |

#### AgentInfo.ActivationKey
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| activationId | String   | &check;      |
| title        | String   | &check;      |

#### AgentInfo.AgentConfiguration
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Long     | &check;      |
| name     | String   | &check;      |

#### AgentInfo.ManifestVersion
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| pc       | String   | &check;      |
| sca      | String   | &check;      |
| vm       | String   | &check;      |

#### AzureAssetSourceSimple
| **Name**          | **Type**                              | **Nullable** |
| ----------------- | ------------------------------------- | ------------ |
| assetId           | String                                | &check;      |
| azureVmTags       | List<AzureAssetSourceSimple.AzureTag> | &check;      |
| firstDiscovered   | String                                | &check;      |
| ipv6              | String                                | &check;      |
| lastUpdated       | String                                | &check;      |
| location          | String                                | &check;      |
| macAddress        | String                                | &check;      |
| name              | String                                | &check;      |
| offer             | String                                | &check;      |
| osType            | String                                | &check;      |
| privateIpAddress  | String                                | &check;      |
| publicIpAddress   | String                                | &check;      |
| publisher         | String                                | &check;      |
| resourceGroupName | String                                | &check;      |
| state             | String                                | &check;      |
| subnet            | String                                | &check;      |
| subscriptionId    | String                                | &check;      |
| type              | String                                | &check;      |
| virtualNetwork    | String                                | &check;      |
| vmId              | String                                | &check;      |
| vmSize            | String                                | &check;      |

#### AzureAssetSourceSimple.AzureTag
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| value    | String   | &check;      |

#### DockerInfo
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| dockerVersion  | String   | &check;      |
| noOfContainers | Int      | &check;      |
| noOfImages     | Int      | &check;      |

#### Ec2AssetSourceSimple
| **Name**          | **Type**                           | **Nullable** |
| ----------------- | ---------------------------------- | ------------ |
| accountId         | String                             | &check;      |
| assetId           | String                             | &check;      |
| availabilityZone  | String                             | &check;      |
| createdDate       | String                             | &check;      |
| ec2InstanceTags   | List<Ec2AssetSourceSimple.EC2Tags> | &check;      |
| firstDiscovered   | String                             | &check;      |
| groupId           | String                             | &check;      |
| groupName         | String                             | &check;      |
| imageId           | String                             | &check;      |
| instanceGroupId   | String                             | &check;      |
| instanceGroupName | String                             | &check;      |
| instanceId        | String                             | &check;      |
| instanceState     | String                             | &check;      |
| instanceType      | String                             | &check;      |
| keyName           | String                             | &check;      |
| lastUpdated       | String                             | &check;      |
| launchTime        | String                             | &check;      |
| localHostname     | String                             | &check;      |
| macAddress        | String                             | &check;      |
| monitoringEnabled | String                             | &check;      |
| privateDnsName    | String                             | &check;      |
| privateIpAddress  | String                             | &check;      |
| publicDnsName     | String                             | &check;      |
| publicIpAddress   | String                             | &check;      |
| region            | String                             | &check;      |
| reservationId     | String                             | &check;      |
| spotInstance      | Boolean                            | &check;      |
| subnetId          | String                             | &check;      |
| type              | String                             | &check;      |
| vpcId             | String                             | &check;      |
| zone              | String                             | &check;      |

#### Ec2AssetSourceSimple.EC2Tags
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| value    | String   | &check;      |

#### GcpAssetSourceSimple
| **Name**         | **Type**                          | **Nullable** |
| ---------------- | --------------------------------- | ------------ |
| assetId          | String                            | &check;      |
| firstDiscovered  | String                            | &check;      |
| gcpInstanceTags  | List<GcpAssetSourceSimple.GCPTag> | &check;      |
| hostname         | String                            | &check;      |
| imageId          | String                            | &check;      |
| instanceId       | String                            | &check;      |
| lastUpdated      | String                            | &check;      |
| macAddress       | String                            | &check;      |
| machineType      | String                            | &check;      |
| network          | String                            | &check;      |
| privateIpAddress | String                            | &check;      |
| projectId        | String                            | &check;      |
| projectIdNo      | String                            | &check;      |
| publicIpAddress  | String                            | &check;      |
| state            | String                            | &check;      |
| type             | String                            | &check;      |
| zone             | String                            | &check;      |

#### GcpAssetSourceSimple.GCPTag
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| key      | String   | &check;      |
| value    | String   | &check;      |

#### HostAssetAccount
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| username | String   | &check;      |

#### HostAssetInterface
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| address        | String   | &check;      |
| gatewayAddress | String   | &check;      |
| hostname       | String   | &check;      |
| interfaceName  | String   | &check;      |
| macAddress     | String   | &check;      |
| type           | String   | &check;      |

#### HostAssetOpenPort
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| port        | Int      | &check;      |
| protocol    | String   | &check;      |
| serviceId   | Long     | &check;      |
| serviceName | String   | &check;      |

#### HostAssetProcessor
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| speed    | Long     | &check;      |

#### HostAssetSoftware
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| version  | String   | &check;      |

#### HostAssetVolume
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| free     | Long     | &check;      |
| name     | String   | &check;      |
| size     | Long     | &check;      |

#### HostAssetVuln
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| firstFound         | String   | &check;      |
| hostInstanceVulnId | String   | &check;      |
| lastFound          | String   | &check;      |
| qid                | String   | &check;      |

#### SourceInfo
| **Name**               | **Type**               | **Nullable** |
| ---------------------- | ---------------------- | ------------ |
| assetSourceSimple      | JSON                   | &check;      |
| azureAssetSourceSimple | AzureAssetSourceSimple | &check;      |
| ec2AssetSourceSimple   | Ec2AssetSourceSimple   | &check;      |
| gcpAssetSourceSimple   | GcpAssetSourceSimple   | &check;      |

#### Tag
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
