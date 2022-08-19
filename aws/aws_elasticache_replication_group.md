---
description: Amazon Web Services ElastiCache Replication Group
---
aws_elasticache_replication_group
---------------------------------

| **Name**                   | **Type**                              | **Nullable** |
| -------------------------- | ------------------------------------- | ------------ |
| accountId                  | String                                | &cross;      |
| accountName                | String                                | &check;      |
| arn                        | String                                | &check;      |
| atRestEncryptionEnabled    | Boolean                               | &check;      |
| authTokenEnabled           | Boolean                               | &check;      |
| authTokenLastModifiedDate  | String                                | &check;      |
| automaticFailover          | String                                | &check;      |
| cacheNodeType              | String                                | &check;      |
| clusterEnabled             | Boolean                               | &check;      |
| configurationEndpoint      | Endpoint                              | &check;      |
| dataTiering                | String                                | &check;      |
| description                | String                                | &check;      |
| globalReplicationGroupInfo | GlobalReplicationGroupInfo            | &check;      |
| kmsKeyId                   | String                                | &check;      |
| logDeliveryConfigurations  | List<LogDeliveryConfiguration>        | &check;      |
| memberClusters             | List<String>                          | &check;      |
| memberClustersOutpostArns  | List<String>                          | &check;      |
| multiAZ                    | String                                | &check;      |
| nodeGroups                 | List<NodeGroup>                       | &check;      |
| pendingModifiedValues      | ReplicationGroupPendingModifiedValues | &check;      |
| region                     | String                                | &cross;      |
| replicationGroupCreateTime | String                                | &check;      |
| replicationGroupId         | String                                | &cross;      |
| snapshotRetentionLimit     | Int                                   | &check;      |
| snapshotWindow             | String                                | &check;      |
| snapshottingClusterId      | String                                | &check;      |
| status                     | String                                | &check;      |
| transitEncryptionEnabled   | Boolean                               | &check;      |
| userGroupIds               | List<String>                          | &check;      |

#### CloudWatchLogsDestinationDetails
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| logGroup | String   | &check;      |

#### DestinationDetails
| **Name**               | **Type**                          | **Nullable** |
| ---------------------- | --------------------------------- | ------------ |
| cloudWatchLogsDetails  | CloudWatchLogsDestinationDetails  | &check;      |
| kinesisFirehoseDetails | KinesisFirehoseDestinationDetails | &check;      |

#### Endpoint
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| address  | String   | &check;      |
| port     | Int      | &check;      |

#### GlobalReplicationGroupInfo
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| globalReplicationGroupId         | String   | &check;      |
| globalReplicationGroupMemberRole | String   | &check;      |

#### KinesisFirehoseDestinationDetails
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| deliveryStream | String   | &check;      |

#### LogDeliveryConfiguration
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| destinationDetails | DestinationDetails | &check;      |
| destinationType    | String             | &check;      |
| logFormat          | String             | &check;      |
| logType            | String             | &check;      |
| message            | String             | &check;      |
| status             | String             | &check;      |

#### NodeGroup
| **Name**         | **Type**              | **Nullable** |
| ---------------- | --------------------- | ------------ |
| nodeGroupId      | String                | &check;      |
| nodeGroupMembers | List<NodeGroupMember> | &check;      |
| primaryEndpoint  | Endpoint              | &check;      |
| readerEndpoint   | Endpoint              | &check;      |
| slots            | String                | &check;      |
| status           | String                | &check;      |

#### NodeGroupMember
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| cacheClusterId            | String   | &check;      |
| cacheNodeId               | String   | &check;      |
| currentRole               | String   | &check;      |
| preferredAvailabilityZone | String   | &check;      |
| preferredOutpostArn       | String   | &check;      |
| readEndpoint              | Endpoint | &check;      |

#### ReplicationGroupPendingModifiedValues
| **Name**                  | **Type**                                                                    | **Nullable** |
| ------------------------- | --------------------------------------------------------------------------- | ------------ |
| authTokenStatus           | String                                                                      | &check;      |
| automaticFailoverStatus   | String                                                                      | &check;      |
| logDeliveryConfigurations | List<ReplicationGroupPendingModifiedValues.PendingLogDeliveryConfiguration> | &check;      |
| primaryClusterId          | String                                                                      | &check;      |
| resharding                | ReplicationGroupPendingModifiedValues.ReshardingStatus                      | &check;      |
| userGroups                | ReplicationGroupPendingModifiedValues.UserGroupsUpdateStatus                | &check;      |

#### ReplicationGroupPendingModifiedValues.PendingLogDeliveryConfiguration
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| destinationDetails | DestinationDetails | &check;      |
| destinationType    | String             | &check;      |
| logFormat          | String             | &check;      |
| logType            | String             | &check;      |

#### ReplicationGroupPendingModifiedValues.ReshardingStatus
| **Name**      | **Type**                                            | **Nullable** |
| ------------- | --------------------------------------------------- | ------------ |
| slotMigration | ReplicationGroupPendingModifiedValues.SlotMigration | &check;      |

#### ReplicationGroupPendingModifiedValues.SlotMigration
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| progressPercentage | Double   | &check;      |

#### ReplicationGroupPendingModifiedValues.UserGroupsUpdateStatus
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| userGroupIdsToAdd    | List<String> | &check;      |
| userGroupIdsToRemove | List<String> | &check;      |
