---
description: Amazon Web Services EMR Cluster
---
aws_emr_cluster
---------------

| **Name**                | **Type**                   | **Nullable** |
| ----------------------- | -------------------------- | ------------ |
| accountId               | String                     | &cross;      |
| accountName             | String                     | &check;      |
| applications            | List<Application>          | &check;      |
| autoScalingRole         | String                     | &check;      |
| autoTerminate           | Boolean                    | &check;      |
| clusterArn              | String                     | &cross;      |
| configurations          | List<Configuration>        | &check;      |
| customAmiId             | String                     | &check;      |
| ebsRootVolumeSize       | Int                        | &check;      |
| ec2InstanceAttributes   | Ec2InstanceAttributes      | &check;      |
| id                      | String                     | &cross;      |
| instanceCollectionType  | String                     | &check;      |
| kerberosAttributes      | KerberosAttributes         | &check;      |
| logEncryptionKmsKeyId   | String                     | &check;      |
| logUri                  | String                     | &check;      |
| masterPublicDnsName     | String                     | &check;      |
| name                    | String                     | &cross;      |
| normalizedInstanceHours | Int                        | &check;      |
| osReleaseLabel          | String                     | &check;      |
| outpostArn              | String                     | &check;      |
| placementGroups         | List<PlacementGroupConfig> | &check;      |
| region                  | String                     | &cross;      |
| releaseLabel            | String                     | &check;      |
| repoUpgradeOnBoot       | String                     | &check;      |
| requestedAmiVersion     | String                     | &check;      |
| runningAmiVersion       | String                     | &check;      |
| scaleDownBehavior       | String                     | &check;      |
| securityConfiguration   | String                     | &check;      |
| serviceRole             | String                     | &check;      |
| status                  | ClusterStatus              | &check;      |
| stepConcurrencyLevel    | Int                        | &check;      |
| tags                    | Map<String,String>         | &check;      |
| terminationProtected    | Boolean                    | &check;      |
| visibleToAllUsers       | Boolean                    | &check;      |

#### Application
| **Name**       | **Type**           | **Nullable** |
| -------------- | ------------------ | ------------ |
| additionalInfo | Map<String,String> | &check;      |
| args           | List<String>       | &check;      |
| name           | String             | &check;      |
| version        | String             | &check;      |

#### ClusterStateChangeReason
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| message  | String   | &check;      |

#### ClusterStatus
| **Name**          | **Type**                 | **Nullable** |
| ----------------- | ------------------------ | ------------ |
| state             | String                   | &check;      |
| stateChangeReason | ClusterStateChangeReason | &check;      |
| timeline          | ClusterTimeline          | &check;      |

#### ClusterTimeline
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| creationDateTime | String   | &check;      |
| endDateTime      | String   | &check;      |
| readyDateTime    | String   | &check;      |

#### Configuration
| **Name**       | **Type**           | **Nullable** |
| -------------- | ------------------ | ------------ |
| classification | String             | &check;      |
| properties     | Map<String,String> | &check;      |

#### Ec2InstanceAttributes
| **Name**                       | **Type**     | **Nullable** |
| ------------------------------ | ------------ | ------------ |
| additionalMasterSecurityGroups | List<String> | &check;      |
| additionalSlaveSecurityGroups  | List<String> | &check;      |
| ec2AvailabilityZone            | String       | &check;      |
| ec2KeyName                     | String       | &check;      |
| ec2SubnetId                    | String       | &check;      |
| emrManagedMasterSecurityGroup  | String       | &check;      |
| emrManagedSlaveSecurityGroup   | String       | &check;      |
| iamInstanceProfile             | String       | &check;      |
| requestedEc2AvailabilityZones  | List<String> | &check;      |
| requestedEc2SubnetIds          | List<String> | &check;      |
| serviceAccessSecurityGroup     | String       | &check;      |

#### KerberosAttributes
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| adDomainJoinPassword             | String   | &check;      |
| adDomainJoinUser                 | String   | &check;      |
| crossRealmTrustPrincipalPassword | String   | &check;      |
| kdcAdminPassword                 | String   | &check;      |
| realm                            | String   | &check;      |

#### PlacementGroupConfig
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| instanceRole      | String   | &check;      |
| placementStrategy | String   | &check;      |
