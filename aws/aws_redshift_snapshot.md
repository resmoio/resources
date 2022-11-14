---
description: Amazon Web Services Redshift Snapshot
---
aws_redshift_snapshot
---------------------

| **Name**                               | **Type**                       | **Nullable** |
| -------------------------------------- | ------------------------------ | ------------ |
| accountId                              | String                         | &cross;      |
| accountName                            | String                         | &check;      |
| accountsWithRestoreAccess              | List<AccountWithRestoreAccess> | &check;      |
| actualIncrementalBackupSizeInMegaBytes | Double                         | &check;      |
| availabilityZone                       | String                         | &check;      |
| backupProgressInMegaBytes              | Double                         | &check;      |
| clusterCreateTime                      | String                         | &check;      |
| clusterIdentifier                      | String                         | &check;      |
| clusterVersion                         | String                         | &check;      |
| currentBackupRateInMegaBytesPerSecond  | Double                         | &check;      |
| dbName                                 | String                         | &check;      |
| elapsedTimeInSeconds                   | Long                           | &check;      |
| encrypted                              | Boolean                        | &check;      |
| encryptedWithHSM                       | Boolean                        | &check;      |
| engineFullVersion                      | String                         | &check;      |
| enhancedVpcRouting                     | Boolean                        | &check;      |
| estimatedSecondsToCompletion           | Long                           | &check;      |
| kmsKeyId                               | String                         | &check;      |
| maintenanceTrackName                   | String                         | &check;      |
| manualSnapshotRemainingDays            | Int                            | &check;      |
| manualSnapshotRetentionPeriod          | Int                            | &check;      |
| masterUsername                         | String                         | &check;      |
| nodeType                               | String                         | &check;      |
| numberOfNodes                          | Int                            | &check;      |
| ownerAccount                           | String                         | &check;      |
| port                                   | Int                            | &check;      |
| region                                 | String                         | &cross;      |
| restorableNodeTypes                    | List<String>                   | &check;      |
| snapshotCreateTime                     | String                         | &check;      |
| snapshotIdentifier                     | String                         | &cross;      |
| snapshotRetentionStartTime             | String                         | &check;      |
| snapshotType                           | String                         | &check;      |
| sourceRegion                           | String                         | &check;      |
| status                                 | String                         | &check;      |
| tags                                   | Map<String,String>             | &check;      |
| totalBackupSizeInMegaBytes             | Double                         | &check;      |
| vpcId                                  | String                         | &check;      |

#### AccountWithRestoreAccess
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| accountAlias | String   | &check;      |
| accountId    | String   | &check;      |
