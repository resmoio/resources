---
description: Amazon Web Services DocumentDB Cluster
---
aws_documentdb_cluster
----------------------

| **Name**                     | **Type**                         | **Nullable** |
| ---------------------------- | -------------------------------- | ------------ |
| accountId                    | String                           | &cross;      |
| accountName                  | String                           | &check;      |
| associatedRoles              | List<DBClusterRole>              | &check;      |
| availabilityZones            | List<String>                     | &check;      |
| backupRetentionPeriod        | Int                              | &check;      |
| clusterCreateTime            | String                           | &check;      |
| dbClusterArn                 | String                           | &check;      |
| dbClusterIdentifier          | String                           | &cross;      |
| dbClusterMembers             | List<DBClusterMember>            | &check;      |
| dbClusterParameterGroup      | String                           | &check;      |
| dbClusterResourceId          | String                           | &check;      |
| dbSubnetGroup                | String                           | &check;      |
| deletionProtection           | Boolean                          | &check;      |
| earliestRestorableTime       | String                           | &check;      |
| enabledCloudwatchLogsExports | List<String>                     | &check;      |
| endpoint                     | String                           | &check;      |
| engine                       | String                           | &check;      |
| engineVersion                | String                           | &check;      |
| hostedZoneId                 | String                           | &check;      |
| kmsKeyId                     | String                           | &check;      |
| masterUsername               | String                           | &check;      |
| multiAZ                      | Boolean                          | &check;      |
| percentProgress              | String                           | &check;      |
| port                         | Int                              | &check;      |
| preferredBackupWindow        | String                           | &check;      |
| preferredMaintenanceWindow   | String                           | &check;      |
| readReplicaIdentifiers       | List<String>                     | &check;      |
| readerEndpoint               | String                           | &check;      |
| region                       | String                           | &cross;      |
| replicationSourceIdentifier  | String                           | &check;      |
| status                       | String                           | &check;      |
| storageEncrypted             | Boolean                          | &check;      |
| vpcSecurityGroups            | List<VpcSecurityGroupMembership> | &check;      |

#### DBClusterMember
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| dbClusterParameterGroupStatus | String   | &check;      |
| dbInstanceIdentifier          | String   | &check;      |
| isClusterWriter               | Boolean  | &check;      |
| promotionTier                 | Int      | &check;      |

#### DBClusterRole
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| roleArn  | String   | &check;      |
| status   | String   | &check;      |

#### VpcSecurityGroupMembership
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| status             | String   | &check;      |
| vpcSecurityGroupId | String   | &check;      |
