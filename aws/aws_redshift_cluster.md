---
description: Amazon Web Services Redshift Cluster
---
aws_redshift_cluster
--------------------

| **Name**                               | **Type**                             | **Nullable** |
| -------------------------------------- | ------------------------------------ | ------------ |
| accountId                              | String                               | &cross;      |
| accountName                            | String                               | &check;      |
| allowVersionUpgrade                    | Boolean                              | &check;      |
| aquaConfiguration                      | AquaConfiguration                    | &check;      |
| automatedSnapshotRetentionPeriod       | Int                                  | &check;      |
| availabilityZone                       | String                               | &check;      |
| availabilityZoneRelocationStatus       | String                               | &check;      |
| clusterAvailabilityStatus              | String                               | &check;      |
| clusterCreateTime                      | String                               | &check;      |
| clusterIdentifier                      | String                               | &cross;      |
| clusterNamespaceArn                    | String                               | &check;      |
| clusterNodes                           | List<ClusterNode>                    | &check;      |
| clusterParameterGroups                 | List<ClusterParameterGroupStatus>    | &check;      |
| clusterPublicKey                       | String                               | &check;      |
| clusterRevisionNumber                  | String                               | &check;      |
| clusterSecurityGroups                  | List<ClusterSecurityGroupMembership> | &check;      |
| clusterSnapshotCopyStatus              | ClusterSnapshotCopyStatus            | &check;      |
| clusterStatus                          | String                               | &check;      |
| clusterSubnetGroupName                 | String                               | &check;      |
| clusterVersion                         | String                               | &check;      |
| dataTransferProgress                   | DataTransferProgress                 | &check;      |
| dbName                                 | String                               | &check;      |
| defaultIamRoleArn                      | String                               | &check;      |
| deferredMaintenanceWindows             | List<DeferredMaintenanceWindow>      | &check;      |
| elasticIpStatus                        | ElasticIpStatus                      | &check;      |
| elasticResizeNumberOfNodeOptions       | String                               | &check;      |
| encrypted                              | Boolean                              | &check;      |
| endpoint                               | Endpoint                             | &check;      |
| enhancedVpcRouting                     | Boolean                              | &check;      |
| expectedNextSnapshotScheduleTime       | String                               | &check;      |
| expectedNextSnapshotScheduleTimeStatus | String                               | &check;      |
| hsmStatus                              | HsmStatus                            | &check;      |
| iamRoles                               | List<ClusterIamRole>                 | &check;      |
| kmsKeyId                               | String                               | &check;      |
| loggingStatus                          | LoggingStatus                        | &check;      |
| maintenanceTrackName                   | String                               | &check;      |
| manualSnapshotRetentionPeriod          | Int                                  | &check;      |
| masterUsername                         | String                               | &check;      |
| modifyStatus                           | String                               | &check;      |
| nextMaintenanceWindowStartTime         | String                               | &check;      |
| nodeType                               | String                               | &check;      |
| numberOfNodes                          | Int                                  | &check;      |
| pendingActions                         | List<String>                         | &check;      |
| pendingModifiedValues                  | PendingModifiedValues                | &check;      |
| preferredMaintenanceWindow             | String                               | &check;      |
| publiclyAccessible                     | Boolean                              | &check;      |
| region                                 | String                               | &cross;      |
| reservedNodeExchangeStatus             | ReservedNodeExchangeStatus           | &check;      |
| resizeInfo                             | ResizeInfo                           | &check;      |
| restoreStatus                          | RestoreStatus                        | &check;      |
| snapshotScheduleIdentifier             | String                               | &check;      |
| snapshotScheduleState                  | String                               | &check;      |
| tags                                   | Map<String,String>                   | &check;      |
| totalStorageCapacityInMegaBytes        | Long                                 | &check;      |
| vpcId                                  | String                               | &check;      |
| vpcSecurityGroups                      | List<VpcSecurityGroupMembership>     | &check;      |

#### AquaConfiguration
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| aquaConfigurationStatus | String   | &check;      |
| aquaStatus              | String   | &check;      |

#### ClusterIamRole
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| applyStatus | String   | &check;      |
| iamRoleArn  | String   | &check;      |

#### ClusterNode
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| nodeRole         | String   | &check;      |
| privateIPAddress | String   | &check;      |
| publicIPAddress  | String   | &check;      |

#### ClusterParameterGroupStatus
| **Name**                   | **Type**                     | **Nullable** |
| -------------------------- | ---------------------------- | ------------ |
| clusterParameterStatusList | List<ClusterParameterStatus> | &check;      |
| parameterApplyStatus       | String                       | &check;      |
| parameterGroupName         | String                       | &check;      |

#### ClusterParameterStatus
| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| parameterApplyErrorDescription | String   | &check;      |
| parameterApplyStatus           | String   | &check;      |
| parameterName                  | String   | &check;      |

#### ClusterSecurityGroupMembership
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| clusterSecurityGroupName | String   | &check;      |
| status                   | String   | &check;      |

#### ClusterSnapshotCopyStatus
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| destinationRegion             | String   | &check;      |
| manualSnapshotRetentionPeriod | Int      | &check;      |
| retentionPeriod               | Long     | &check;      |
| snapshotCopyGrantName         | String   | &check;      |

#### DataTransferProgress
| **Name**                           | **Type** | **Nullable** |
| ---------------------------------- | -------- | ------------ |
| currentRateInMegaBytesPerSecond    | Double   | &check;      |
| dataTransferredInMegaBytes         | Long     | &check;      |
| elapsedTimeInSeconds               | Long     | &check;      |
| estimatedTimeToCompletionInSeconds | Long     | &check;      |
| status                             | String   | &check;      |
| totalDataInMegaBytes               | Long     | &check;      |

#### DeferredMaintenanceWindow
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| deferMaintenanceEndTime    | String   | &check;      |
| deferMaintenanceIdentifier | String   | &check;      |
| deferMaintenanceStartTime  | String   | &check;      |

#### ElasticIpStatus
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| elasticIp | String   | &check;      |
| status    | String   | &check;      |

#### Endpoint
| **Name**     | **Type**          | **Nullable** |
| ------------ | ----------------- | ------------ |
| address      | String            | &check;      |
| port         | Int               | &check;      |
| vpcEndpoints | List<VpcEndpoint> | &check;      |

#### HsmStatus
| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| hsmClientCertificateIdentifier | String   | &check;      |
| hsmConfigurationIdentifier     | String   | &check;      |
| status                         | String   | &check;      |

#### LoggingStatus
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| bucketName         | String       | &check;      |
| logDestinationType | String       | &check;      |
| logExports         | List<String> | &check;      |
| loggingEnabled     | Boolean      | &check;      |
| s3KeyPrefix        | String       | &check;      |

#### NetworkInterface
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| availabilityZone   | String   | &check;      |
| networkInterfaceId | String   | &check;      |
| privateIpAddress   | String   | &check;      |
| subnetId           | String   | &check;      |

#### PendingModifiedValues
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| automatedSnapshotRetentionPeriod | Int      | &check;      |
| clusterIdentifier                | String   | &check;      |
| clusterType                      | String   | &check;      |
| clusterVersion                   | String   | &check;      |
| encryptionType                   | String   | &check;      |
| enhancedVpcRouting               | Boolean  | &check;      |
| maintenanceTrackName             | String   | &check;      |
| masterUserPassword               | String   | &check;      |
| nodeType                         | String   | &check;      |
| numberOfNodes                    | Int      | &check;      |
| publiclyAccessible               | Boolean  | &check;      |

#### ReservedNodeExchangeStatus
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| requestTime                   | String   | &check;      |
| reservedNodeExchangeRequestId | String   | &check;      |
| sourceReservedNodeCount       | Int      | &check;      |
| sourceReservedNodeId          | String   | &check;      |
| sourceReservedNodeType        | String   | &check;      |
| status                        | String   | &check;      |
| targetReservedNodeCount       | Int      | &check;      |
| targetReservedNodeOfferingId  | String   | &check;      |
| targetReservedNodeType        | String   | &check;      |

#### ResizeInfo
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| allowCancelResize | Boolean  | &check;      |
| resizeType        | String   | &check;      |

#### RestoreStatus
| **Name**                               | **Type** | **Nullable** |
| -------------------------------------- | -------- | ------------ |
| currentRestoreRateInMegaBytesPerSecond | Double   | &check;      |
| elapsedTimeInSeconds                   | Long     | &check;      |
| estimatedTimeToCompletionInSeconds     | Long     | &check;      |
| progressInMegaBytes                    | Long     | &check;      |
| snapshotSizeInMegaBytes                | Long     | &check;      |
| status                                 | String   | &check;      |

#### VpcEndpoint
| **Name**          | **Type**               | **Nullable** |
| ----------------- | ---------------------- | ------------ |
| networkInterfaces | List<NetworkInterface> | &check;      |
| vpcEndpointId     | String                 | &check;      |
| vpcId             | String                 | &check;      |

#### VpcSecurityGroupMembership
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| status             | String   | &check;      |
| vpcSecurityGroupId | String   | &check;      |
