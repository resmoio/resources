---
description: Amazon Web Services ElastiCache Cluster
---
aws_elasticache_cluster
-----------------------

| **Name**                           | **Type**                           | **Nullable** |
| ---------------------------------- | ---------------------------------- | ------------ |
| accountId                          | String                             | &cross;      |
| accountName                        | String                             | &check;      |
| arn                                | String                             | &check;      |
| atRestEncryptionEnabled            | Boolean                            | &check;      |
| authTokenEnabled                   | Boolean                            | &check;      |
| authTokenLastModifiedDate          | String                             | &check;      |
| autoMinorVersionUpgrade            | Boolean                            | &check;      |
| cacheClusterCreateTime             | String                             | &check;      |
| cacheClusterId                     | String                             | &cross;      |
| cacheClusterStatus                 | String                             | &check;      |
| cacheNodeType                      | String                             | &check;      |
| cacheNodes                         | List<CacheNode>                    | &check;      |
| cacheParameterGroup                | CacheParameterGroupStatus          | &check;      |
| cacheSecurityGroups                | List<CacheSecurityGroupMembership> | &check;      |
| cacheSubnetGroupName               | String                             | &check;      |
| clientDownloadLandingPage          | String                             | &check;      |
| configurationEndpoint              | Endpoint                           | &check;      |
| engine                             | String                             | &check;      |
| engineVersion                      | String                             | &check;      |
| logDeliveryConfigurations          | List<LogDeliveryConfiguration>     | &check;      |
| notificationConfiguration          | NotificationConfiguration          | &check;      |
| numCacheNodes                      | Int                                | &check;      |
| pendingModifiedValues              | PendingModifiedValues              | &check;      |
| preferredAvailabilityZone          | String                             | &check;      |
| preferredMaintenanceWindow         | String                             | &check;      |
| preferredOutpostArn                | String                             | &check;      |
| region                             | String                             | &cross;      |
| replicationGroupId                 | String                             | &check;      |
| replicationGroupLogDeliveryEnabled | Boolean                            | &check;      |
| securityGroups                     | List<SecurityGroupMembership>      | &check;      |
| snapshotRetentionLimit             | Int                                | &check;      |
| snapshotWindow                     | String                             | &check;      |
| transitEncryptionEnabled           | Boolean                            | &check;      |

#### CacheNode
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| cacheNodeCreateTime      | String   | &check;      |
| cacheNodeId              | String   | &check;      |
| cacheNodeStatus          | String   | &check;      |
| customerAvailabilityZone | String   | &check;      |
| customerOutpostArn       | String   | &check;      |
| endpoint                 | Endpoint | &check;      |
| parameterGroupStatus     | String   | &check;      |
| sourceCacheNodeId        | String   | &check;      |

#### CacheParameterGroupStatus
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| cacheNodeIdsToReboot    | List<String> | &check;      |
| cacheParameterGroupName | String       | &check;      |
| parameterApplyStatus    | String       | &check;      |

#### CacheSecurityGroupMembership
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| cacheSecurityGroupName | String   | &check;      |
| status                 | String   | &check;      |

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

#### NotificationConfiguration
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| topicArn    | String   | &check;      |
| topicStatus | String   | &check;      |

#### PendingModifiedValues
| **Name**                  | **Type**                                                    | **Nullable** |
| ------------------------- | ----------------------------------------------------------- | ------------ |
| authTokenStatus           | String                                                      | &check;      |
| cacheNodeIdsToRemove      | List<String>                                                | &check;      |
| cacheNodeType             | String                                                      | &check;      |
| engineVersion             | String                                                      | &check;      |
| logDeliveryConfigurations | List<PendingModifiedValues.PendingLogDeliveryConfiguration> | &check;      |
| numCacheNodes             | Int                                                         | &check;      |

#### PendingModifiedValues.PendingLogDeliveryConfiguration
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| destinationDetails | DestinationDetails | &check;      |
| destinationType    | String             | &check;      |
| logFormat          | String             | &check;      |
| logType            | String             | &check;      |

#### SecurityGroupMembership
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| securityGroupId | String   | &check;      |
| status          | String   | &check;      |
