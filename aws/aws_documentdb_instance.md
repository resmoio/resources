---
description: Amazon Web Services DocumentDB Instance
---
aws_documentdb_instance
-----------------------

| **Name**                     | **Type**                         | **Nullable** |
| ---------------------------- | -------------------------------- | ------------ |
| accountId                    | String                           | &cross;      |
| accountName                  | String                           | &check;      |
| autoMinorVersionUpgrade      | Boolean                          | &check;      |
| availabilityZone             | String                           | &check;      |
| backupRetentionPeriod        | Int                              | &check;      |
| caCertificateIdentifier      | String                           | &check;      |
| dbClusterIdentifier          | String                           | &check;      |
| dbInstanceArn                | String                           | &check;      |
| dbInstanceClass              | String                           | &check;      |
| dbInstanceIdentifier         | String                           | &cross;      |
| dbInstanceStatus             | String                           | &check;      |
| dbSubnetGroup                | DBSubnetGroup                    | &check;      |
| dbiResourceId                | String                           | &check;      |
| enabledCloudwatchLogsExports | List<String>                     | &check;      |
| endpoint                     | Endpoint                         | &check;      |
| engine                       | String                           | &check;      |
| engineVersion                | String                           | &check;      |
| instanceCreateTime           | String                           | &check;      |
| kmsKeyId                     | String                           | &check;      |
| pendingModifiedValues        | PendingModifiedValues            | &check;      |
| preferredBackupWindow        | String                           | &check;      |
| preferredMaintenanceWindow   | String                           | &check;      |
| promotionTier                | Int                              | &check;      |
| publiclyAccessible           | Boolean                          | &check;      |
| region                       | String                           | &cross;      |
| statusInfos                  | List<DBInstanceStatusInfo>       | &check;      |
| storageEncrypted             | Boolean                          | &check;      |
| vpcSecurityGroups            | List<VpcSecurityGroupMembership> | &check;      |

#### DBInstanceStatusInfo
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| message    | String   | &check;      |
| normal     | Boolean  | &check;      |
| status     | String   | &check;      |
| statusType | String   | &check;      |

#### DBSubnetGroup
| **Name**                 | **Type**                   | **Nullable** |
| ------------------------ | -------------------------- | ------------ |
| dbSubnetGroupArn         | String                     | &check;      |
| dbSubnetGroupDescription | String                     | &check;      |
| dbSubnetGroupName        | String                     | &check;      |
| subnetGroupStatus        | String                     | &check;      |
| subnets                  | List<DBSubnetGroup.Subnet> | &check;      |
| vpcId                    | String                     | &check;      |

#### DBSubnetGroup.AvailabilityZone
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |

#### DBSubnetGroup.Subnet
| **Name**               | **Type**                       | **Nullable** |
| ---------------------- | ------------------------------ | ------------ |
| subnetAvailabilityZone | DBSubnetGroup.AvailabilityZone | &check;      |
| subnetIdentifier       | String                         | &check;      |
| subnetStatus           | String                         | &check;      |

#### Endpoint
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| address      | String   | &check;      |
| hostedZoneId | String   | &check;      |
| port         | Int      | &check;      |

#### PendingCloudwatchLogsExports
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| logTypesToDisable | List<String> | &check;      |
| logTypesToEnable  | List<String> | &check;      |

#### PendingModifiedValues
| **Name**                     | **Type**                     | **Nullable** |
| ---------------------------- | ---------------------------- | ------------ |
| allocatedStorage             | Int                          | &check;      |
| backupRetentionPeriod        | Int                          | &check;      |
| caCertificateIdentifier      | String                       | &check;      |
| dbInstanceClass              | String                       | &check;      |
| dbInstanceIdentifier         | String                       | &check;      |
| dbSubnetGroupName            | String                       | &check;      |
| engineVersion                | String                       | &check;      |
| iops                         | Int                          | &check;      |
| licenseModel                 | String                       | &check;      |
| masterUserPassword           | String                       | &check;      |
| multiAZ                      | Boolean                      | &check;      |
| pendingCloudwatchLogsExports | PendingCloudwatchLogsExports | &check;      |
| port                         | Int                          | &check;      |
| storageType                  | String                       | &check;      |

#### VpcSecurityGroupMembership
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| status             | String   | &check;      |
| vpcSecurityGroupId | String   | &check;      |
