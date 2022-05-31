---
description: Amazon Web Services Backup Plan
---
aws_backup_plan
---------------

| **Name**               | **Type**                    | **Nullable** |
| ---------------------- | --------------------------- | ------------ |
| accountId              | String                      | &cross;      |
| advancedBackupSettings | List<AdvancedBackupSetting> | &check;      |
| arn                    | String                      | &cross;      |
| creationDate           | String                      | &check;      |
| creatorRequestId       | String                      | &check;      |
| deletionDate           | String                      | &check;      |
| id                     | String                      | &cross;      |
| lastExecutionDate      | String                      | &check;      |
| name                   | String                      | &cross;      |
| region                 | String                      | &cross;      |
| rules                  | List<BackupRule>            | &cross;      |
| tags                   | Map<String,String>          | &cross;      |
| versionId              | String                      | &cross;      |

#### AdvancedBackupSetting
| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| backupOptions | Map<String,String> | &check;      |
| resourceType  | String             | &cross;      |

#### BackupRule
| **Name**                | **Type**                    | **Nullable** |
| ----------------------- | --------------------------- | ------------ |
| completionWindowMinutes | Long                        | &cross;      |
| copyActions             | List<BackupRule.CopyAction> | &check;      |
| enableContinuousBackup  | Boolean                     | &check;      |
| lifecycle               | BackupRule.Lifecycle        | &check;      |
| recoveryPointTags       | Map<String,String>          | &check;      |
| ruleId                  | String                      | &cross;      |
| ruleName                | String                      | &cross;      |
| scheduleExpression      | String                      | &cross;      |
| startWindowMinutes      | Long                        | &cross;      |
| targetBackupVaultName   | String                      | &cross;      |

#### BackupRule.CopyAction
| **Name**                  | **Type**             | **Nullable** |
| ------------------------- | -------------------- | ------------ |
| destinationBackupVaultArn | String               | &cross;      |
| lifecycle                 | BackupRule.Lifecycle | &check;      |

#### BackupRule.Lifecycle
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| deleteAfterDays            | Long     | &cross;      |
| moveToColdStorageAfterDays | Long     | &check;      |
