---
description: Amazon Web Services EC2 Launch Template
---
aws_ec2_launch_template
-----------------------

| **Name**             | **Type**                    | **Nullable** |
| -------------------- | --------------------------- | ------------ |
| accountId            | String                      | &cross;      |
| createTime           | String                      | &check;      |
| createdBy            | String                      | &check;      |
| defaultVersionNumber | Long                        | &check;      |
| latestVersionNumber  | Long                        | &check;      |
| launchTemplateId     | String                      | &cross;      |
| launchTemplateName   | String                      | &cross;      |
| region               | String                      | &cross;      |
| tags                 | Map<String,String>          | &check;      |
| versions             | List<LaunchTemplateVersion> | &check;      |

#### LaunchTemplateBlockDeviceMapping
| **Name**    | **Type**                             | **Nullable** |
| ----------- | ------------------------------------ | ------------ |
| deviceName  | String                               | &check;      |
| ebs         | LaunchTemplateBlockDeviceMapping.Ebs | &check;      |
| noDevice    | String                               | &check;      |
| virtualName | String                               | &check;      |

#### LaunchTemplateBlockDeviceMapping.Ebs
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| deleteOnTermination | Boolean  | &check;      |
| encrypted           | Boolean  | &check;      |
| iops                | Int      | &check;      |
| kmsKeyId            | String   | &check;      |
| snapshotId          | String   | &check;      |
| throughput          | Int      | &check;      |
| volumeSize          | Int      | &check;      |
| volumeType          | String   | &check;      |

#### LaunchTemplateCpuOptions
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| coreCount      | Int      | &check;      |
| threadsPerCore | Int      | &check;      |

#### LaunchTemplateElasticInferenceAcceleratorResponse
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| count    | Int      | &check;      |
| type     | String   | &check;      |

#### LaunchTemplateInstanceMetadataOptions
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| httpEndpoint            | String   | &check;      |
| httpProtocolIpv6        | String   | &check;      |
| httpPutResponseHopLimit | Int      | &check;      |
| httpTokens              | String   | &check;      |
| state                   | String   | &check;      |

#### LaunchTemplateInstanceNetworkInterfaceSpecification
| **Name**                       | **Type**     | **Nullable** |
| ------------------------------ | ------------ | ------------ |
| associateCarrierIpAddress      | Boolean      | &check;      |
| associatePublicIpAddress       | Boolean      | &check;      |
| deleteOnTermination            | Boolean      | &check;      |
| description                    | String       | &check;      |
| deviceIndex                    | Int          | &check;      |
| groups                         | List<String> | &check;      |
| interfaceType                  | String       | &check;      |
| ipv4PrefixCount                | Int          | &check;      |
| ipv4Prefixes                   | List<String> | &check;      |
| ipv6AddressCount               | Int          | &check;      |
| ipv6Addresses                  | List<String> | &check;      |
| ipv6PrefixCount                | Int          | &check;      |
| ipv6Prefixes                   | List<String> | &check;      |
| networkCardIndex               | Int          | &check;      |
| networkInterfaceId             | String       | &check;      |
| privateIpAddress               | String       | &check;      |
| privateIpAddresses             | List<String> | &check;      |
| secondaryPrivateIpAddressCount | Int          | &check;      |
| subnetId                       | String       | &check;      |

#### LaunchTemplatePlacement
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| affinity             | String   | &check;      |
| availabilityZone     | String   | &check;      |
| groupName            | String   | &check;      |
| hostId               | String   | &check;      |
| hostResourceGroupArn | String   | &check;      |
| partitionNumber      | Int      | &check;      |
| spreadDomain         | String   | &check;      |
| tenancy              | String   | &check;      |

#### LaunchTemplatePrivateDnsNameOptions
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| enableResourceNameDnsAAAARecord | Boolean  | &check;      |
| enableResourceNameDnsARecord    | Boolean  | &check;      |
| hostnameType                    | String   | &check;      |

#### LaunchTemplateTagSpecification
| **Name**     | **Type**           | **Nullable** |
| ------------ | ------------------ | ------------ |
| resourceType | String             | &check;      |
| tags         | Map<String,String> | &check;      |

#### LaunchTemplateVersion
| **Name**           | **Type**                   | **Nullable** |
| ------------------ | -------------------------- | ------------ |
| createTime         | String                     | &check;      |
| createdBy          | String                     | &check;      |
| defaultVersion     | Boolean                    | &check;      |
| launchTemplateData | ResponseLaunchTemplateData | &check;      |
| launchTemplateId   | String                     | &check;      |
| launchTemplateName | String                     | &check;      |
| versionDescription | String                     | &check;      |
| versionNumber      | Long                       | &check;      |

#### ResponseLaunchTemplateData
| **Name**                          | **Type**                                                  | **Nullable** |
| --------------------------------- | --------------------------------------------------------- | ------------ |
| blockDeviceMappings               | List<LaunchTemplateBlockDeviceMapping>                    | &check;      |
| cpuOptions                        | LaunchTemplateCpuOptions                                  | &check;      |
| creditSpecification               | String                                                    | &check;      |
| disableApiTermination             | Boolean                                                   | &check;      |
| ebsOptimized                      | Boolean                                                   | &check;      |
| elasticGpuSpecifications          | List<String>                                              | &check;      |
| elasticInferenceAccelerators      | List<LaunchTemplateElasticInferenceAcceleratorResponse>   | &check;      |
| enclaveOptions                    | Boolean                                                   | &check;      |
| hibernationOptions                | Boolean                                                   | &check;      |
| iamInstanceProfile                | String                                                    | &check;      |
| imageId                           | String                                                    | &check;      |
| instanceInitiatedShutdownBehavior | String                                                    | &check;      |
| instanceType                      | String                                                    | &check;      |
| kernelId                          | String                                                    | &check;      |
| keyName                           | String                                                    | &check;      |
| licenseSpecifications             | List<String>                                              | &check;      |
| metadataOptions                   | LaunchTemplateInstanceMetadataOptions                     | &check;      |
| monitoring                        | Boolean                                                   | &check;      |
| networkInterfaces                 | List<LaunchTemplateInstanceNetworkInterfaceSpecification> | &check;      |
| placement                         | LaunchTemplatePlacement                                   | &check;      |
| privateDnsNameOptions             | LaunchTemplatePrivateDnsNameOptions                       | &check;      |
| ramDiskId                         | String                                                    | &check;      |
| securityGroupIds                  | List<String>                                              | &check;      |
| securityGroups                    | List<String>                                              | &check;      |
| tagSpecifications                 | List<LaunchTemplateTagSpecification>                      | &check;      |
| userData                          | String                                                    | &check;      |
