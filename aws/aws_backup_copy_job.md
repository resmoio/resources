---
description: Amazon Web Services Backup Copy Job
---
aws_backup_copy_job
-------------------

| **Name**                    | **Type**             | **Nullable** |
| --------------------------- | -------------------- | ------------ |
| accountId                   | String               | &cross;      |
| accountName                 | String               | &check;      |
| backupSizeInBytes           | Long                 | &check;      |
| completionDate              | String               | &check;      |
| copyJobAccountId            | String               | &cross;      |
| createdBy                   | RecoveryPointCreator | &check;      |
| creationDate                | String               | &check;      |
| destinationBackupVaultArn   | String               | &check;      |
| destinationRecoveryPointArn | String               | &check;      |
| iamRoleArn                  | String               | &cross;      |
| id                          | String               | &cross;      |
| region                      | String               | &cross;      |
| resourceArn                 | String               | &cross;      |
| resourceType                | String               | &cross;      |
| sourceBackupVaultArn        | String               | &cross;      |
| sourceRecoveryPointArn      | String               | &cross;      |
| state                       | String               | &cross;      |
| statusMessage               | String               | &check;      |

#### RecoveryPointCreator
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| backupPlanArn     | String   | &check;      |
| backupPlanId      | String   | &check;      |
| backupPlanVersion | String   | &check;      |
| backupRuleId      | String   | &check;      |
