---
description: Amazon Web Services RDS Instance
---
aws_rds_instance
----------------

| **Name**                                      | **Type**                         | **Nullable** |
| --------------------------------------------- | -------------------------------- | ------------ |
| accountId                                     | String                           | &cross;      |
| accountName                                   | String                           | &check;      |
| activityStreamEngineNativeAuditFieldsIncluded | Boolean                          | &check;      |
| activityStreamKinesisStreamName               | String                           | &check;      |
| activityStreamKmsKeyId                        | String                           | &check;      |
| activityStreamMode                            | String                           | &check;      |
| activityStreamStatus                          | String                           | &check;      |
| allocatedStorage                              | Int                              | &check;      |
| arn                                           | String                           | &cross;      |
| associatedRoles                               | List<DBInstanceRole>             | &check;      |
| autoMinorVersionUpgrade                       | Boolean                          | &check;      |
| automaticRestartTime                          | String                           | &check;      |
| automationMode                                | String                           | &check;      |
| availabilityZone                              | String                           | &check;      |
| awsBackupRecoveryPointArn                     | String                           | &check;      |
| backupRetentionPeriod                         | Int                              | &check;      |
| backupTarget                                  | String                           | &check;      |
| caCertificateIdentifier                       | String                           | &check;      |
| characterSetName                              | String                           | &check;      |
| copyTagsToSnapshot                            | Boolean                          | &check;      |
| customIamInstanceProfile                      | String                           | &check;      |
| customerOwnedIpEnabled                        | Boolean                          | &check;      |
| dbClusterIdentifier                           | String                           | &check;      |
| dbInstanceAutomatedBackupsReplications        | List<String>                     | &check;      |
| dbInstanceClass                               | String                           | &check;      |
| dbInstancePort                                | Int                              | &check;      |
| dbInstanceStatus                              | String                           | &check;      |
| dbName                                        | String                           | &check;      |
| dbParameterGroups                             | List<DBParameterGroupStatus>     | &check;      |
| dbSecurityGroups                              | List<DBSecurityGroupMembership>  | &check;      |
| dbSubnetGroup                                 | DBSubnetGroup                    | &check;      |
| dbiResourceId                                 | String                           | &check;      |
| deletionProtection                            | Boolean                          | &check;      |
| domainMemberships                             | List<DomainMembership>           | &check;      |
| enabledCloudwatchLogsExports                  | List<String>                     | &check;      |
| endpoint                                      | Endpoint                         | &check;      |
| engine                                        | String                           | &check;      |
| engineVersion                                 | String                           | &check;      |
| enhancedMonitoringResourceArn                 | String                           | &check;      |
| iamDatabaseAuthenticationEnabled              | Boolean                          | &check;      |
| id                                            | String                           | &cross;      |
| instanceCreateTime                            | String                           | &check;      |
| iops                                          | Int                              | &check;      |
| kmsKeyId                                      | String                           | &check;      |
| licenseModel                                  | String                           | &check;      |
| listenerEndpoint                              | Endpoint                         | &check;      |
| masterUsername                                | String                           | &check;      |
| maxAllocatedStorage                           | Int                              | &check;      |
| monitoringInterval                            | Int                              | &check;      |
| monitoringRoleArn                             | String                           | &check;      |
| multiAZ                                       | Boolean                          | &check;      |
| ncharCharacterSetName                         | String                           | &check;      |
| optionGroupMemberships                        | List<OptionGroupMembership>      | &check;      |
| pendingModifiedValues                         | PendingModifiedValues            | &check;      |
| performanceInsightsEnabled                    | Boolean                          | &check;      |
| performanceInsightsKMSKeyId                   | String                           | &check;      |
| performanceInsightsRetentionPeriod            | Int                              | &check;      |
| preferredBackupWindow                         | String                           | &check;      |
| preferredMaintenanceWindow                    | String                           | &check;      |
| processorFeatures                             | Map<String,String>               | &check;      |
| promotionTier                                 | Int                              | &check;      |
| publiclyAccessible                            | Boolean                          | &check;      |
| readReplicaDBClusterIdentifiers               | List<String>                     | &check;      |
| readReplicaDBInstanceIdentifiers              | List<String>                     | &check;      |
| readReplicaSourceDBInstanceIdentifier         | String                           | &check;      |
| region                                        | String                           | &cross;      |
| replicaMode                                   | String                           | &check;      |
| resumeFullAutomationModeTime                  | String                           | &check;      |
| secondaryAvailabilityZone                     | String                           | &check;      |
| statusInfos                                   | List<DBInstanceStatusInfo>       | &check;      |
| storageEncrypted                              | Boolean                          | &check;      |
| storageType                                   | String                           | &check;      |
| tagList                                       | Map<String,String>               | &check;      |
| tdeCredentialArn                              | String                           | &check;      |
| timezone                                      | String                           | &check;      |
| vpcSecurityGroups                             | List<VpcSecurityGroupMembership> | &check;      |

#### DBInstanceRole
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| featureName | String   | &check;      |
| roleArn     | String   | &cross;      |
| status      | String   | &check;      |

#### DBInstanceStatusInfo
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| message    | String   | &check;      |
| normal     | Boolean  | &check;      |
| status     | String   | &check;      |
| statusType | String   | &check;      |

#### DBParameterGroupStatus
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| dbParameterGroupName | String   | &cross;      |
| parameterApplyStatus | String   | &check;      |

#### DBSecurityGroupMembership
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| dbSecurityGroupName | String   | &cross;      |
| status              | String   | &check;      |

#### DBSubnetGroup
| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| dbSubnetGroupArn         | String       | &check;      |
| dbSubnetGroupDescription | String       | &check;      |
| dbSubnetGroupName        | String       | &cross;      |
| subnetGroupStatus        | String       | &check;      |
| subnets                  | List<String> | &check;      |
| vpcId                    | String       | &check;      |

#### DomainMembership
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| domain      | String   | &check;      |
| fqdn        | String   | &check;      |
| iamRoleName | String   | &check;      |
| status      | String   | &check;      |

#### Endpoint
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| address      | String   | &check;      |
| hostedZoneId | String   | &check;      |
| port         | Int      | &check;      |

#### OptionGroupMembership
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| optionGroupName | String   | &cross;      |
| status          | String   | &check;      |

#### PendingModifiedValues
| **Name**                         | **Type**                                           | **Nullable** |
| -------------------------------- | -------------------------------------------------- | ------------ |
| allocatedStorage                 | Int                                                | &check;      |
| automationMode                   | String                                             | &check;      |
| backupRetentionPeriod            | Int                                                | &check;      |
| caCertificateIdentifier          | String                                             | &check;      |
| dbInstanceClass                  | String                                             | &check;      |
| dbInstanceIdentifier             | String                                             | &check;      |
| dbSubnetGroupName                | String                                             | &check;      |
| engineVersion                    | String                                             | &check;      |
| iamDatabaseAuthenticationEnabled | Boolean                                            | &check;      |
| iops                             | Int                                                | &check;      |
| licenseModel                     | String                                             | &check;      |
| masterUserPassword               | String                                             | &check;      |
| multiAZ                          | Boolean                                            | &check;      |
| pendingCloudwatchLogsExports     | PendingModifiedValues.PendingCloudwatchLogsExports | &check;      |
| port                             | Int                                                | &check;      |
| processorFeatures                | Map<String,String>                                 | &check;      |
| resumeFullAutomationModeTime     | String                                             | &check;      |
| storageType                      | String                                             | &check;      |

#### PendingModifiedValues.PendingCloudwatchLogsExports
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| logTypesToDisable | List<String> | &check;      |
| logTypesToEnable  | List<String> | &check;      |

#### VpcSecurityGroupMembership
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| status             | String   | &check;      |
| vpcSecurityGroupId | String   | &cross;      |
