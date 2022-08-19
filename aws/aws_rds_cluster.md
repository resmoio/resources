---
description: Amazon Web Services RDS Cluster
---
aws_rds_cluster
---------------

| **Name**                           | **Type**                         | **Nullable** |
| ---------------------------------- | -------------------------------- | ------------ |
| accountId                          | String                           | &cross;      |
| accountName                        | String                           | &check;      |
| activityStreamKinesisStreamName    | String                           | &check;      |
| activityStreamKmsKeyId             | String                           | &check;      |
| activityStreamMode                 | String                           | &check;      |
| activityStreamStatus               | String                           | &check;      |
| allocatedStorage                   | Int                              | &check;      |
| arn                                | String                           | &cross;      |
| associatedRoles                    | List<DBClusterRole>              | &check;      |
| autoMinorVersionUpgrade            | Boolean                          | &check;      |
| automaticRestartTime               | String                           | &check;      |
| availabilityZones                  | List<String>                     | &check;      |
| backtrackConsumedChangeRecords     | Long                             | &check;      |
| backtrackWindow                    | Long                             | &check;      |
| backupRetentionPeriod              | Int                              | &check;      |
| capacity                           | Int                              | &check;      |
| characterSetName                   | String                           | &check;      |
| cloneGroupId                       | String                           | &check;      |
| clusterCreateTime                  | String                           | &check;      |
| copyTagsToSnapshot                 | Boolean                          | &check;      |
| crossAccountClone                  | Boolean                          | &check;      |
| customEndpoints                    | List<String>                     | &check;      |
| dbClusterInstanceClass             | String                           | &check;      |
| dbClusterMembers                   | List<DBClusterMember>            | &check;      |
| dbClusterOptionGroupMemberships    | List<DBClusterOptionGroupStatus> | &check;      |
| dbClusterParameterGroup            | String                           | &check;      |
| dbClusterResourceId                | String                           | &check;      |
| dbSubnetGroup                      | String                           | &check;      |
| deletionProtection                 | Boolean                          | &check;      |
| domainMemberships                  | List<DomainMembership>           | &check;      |
| enabledCloudwatchLogsExports       | List<String>                     | &check;      |
| endpoint                           | String                           | &check;      |
| engine                             | String                           | &check;      |
| engineMode                         | String                           | &check;      |
| engineVersion                      | String                           | &check;      |
| globalWriteForwardingRequested     | Boolean                          | &check;      |
| globalWriteForwardingStatus        | String                           | &check;      |
| hostedZoneId                       | String                           | &check;      |
| httpEndpointEnabled                | Boolean                          | &check;      |
| iamDatabaseAuthenticationEnabled   | Boolean                          | &check;      |
| id                                 | String                           | &cross;      |
| iops                               | Int                              | &check;      |
| kmsKeyId                           | String                           | &check;      |
| masterUsername                     | String                           | &check;      |
| monitoringInterval                 | Int                              | &check;      |
| monitoringRoleArn                  | String                           | &check;      |
| multiAZ                            | Boolean                          | &check;      |
| name                               | String                           | &check;      |
| pendingModifiedValues              | ClusterPendingModifiedValues     | &check;      |
| percentProgress                    | String                           | &check;      |
| performanceInsightsEnabled         | Boolean                          | &check;      |
| performanceInsightsKMSKeyId        | String                           | &check;      |
| performanceInsightsRetentionPeriod | Int                              | &check;      |
| port                               | Int                              | &check;      |
| preferredBackupWindow              | String                           | &check;      |
| preferredMaintenanceWindow         | String                           | &check;      |
| publiclyAccessible                 | Boolean                          | &check;      |
| readReplicaIdentifiers             | List<String>                     | &check;      |
| readerEndpoint                     | String                           | &check;      |
| region                             | String                           | &cross;      |
| replicationSourceIdentifier        | String                           | &check;      |
| scalingConfigurationInfo           | ScalingConfigurationInfo         | &check;      |
| status                             | String                           | &check;      |
| storageEncrypted                   | Boolean                          | &check;      |
| storageType                        | String                           | &check;      |
| tagList                            | Map<String,String>               | &check;      |
| vpcSecurityGroups                  | List<VpcSecurityGroupMembership> | &check;      |

#### ClusterPendingModifiedValues
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| dbClusterIdentifier              | String   | &check;      |
| engineVersion                    | String   | &check;      |
| iamDatabaseAuthenticationEnabled | Boolean  | &check;      |
| masterUserPassword               | String   | &check;      |

#### DBClusterMember
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| dbClusterParameterGroupStatus | String   | &check;      |
| dbInstanceIdentifier          | String   | &cross;      |
| isClusterWriter               | Boolean  | &check;      |
| promotionTier                 | Int      | &check;      |

#### DBClusterOptionGroupStatus
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| dbClusterOptionGroupName | String   | &cross;      |
| status                   | String   | &check;      |

#### DBClusterRole
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| featureName | String   | &check;      |
| roleArn     | String   | &cross;      |
| status      | String   | &check;      |

#### DomainMembership
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| domain      | String   | &check;      |
| fqdn        | String   | &check;      |
| iamRoleName | String   | &check;      |
| status      | String   | &check;      |

#### ScalingConfigurationInfo
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| autoPause             | Boolean  | &check;      |
| maxCapacity           | Int      | &check;      |
| minCapacity           | Int      | &check;      |
| secondsBeforeTimeout  | Int      | &check;      |
| secondsUntilAutoPause | Int      | &check;      |
| timeoutAction         | String   | &check;      |

#### VpcSecurityGroupMembership
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| status             | String   | &check;      |
| vpcSecurityGroupId | String   | &cross;      |
