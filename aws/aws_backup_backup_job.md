---
description: Amazon Web Services Backup Job
---
aws_backup_backup_job
---------------------

| **Name**               | **Type**             | **Nullable** |
| ---------------------- | -------------------- | ------------ |
| accountId              | String               | &cross;      |
| accountName            | String               | &check;      |
| backupJobAccountId     | String               | &cross;      |
| backupOptions          | Map<String,String>   | &check;      |
| backupSizeInBytes      | Long                 | &check;      |
| backupType             | String               | &check;      |
| backupVaultArn         | String               | &cross;      |
| backupVaultName        | String               | &cross;      |
| bytesTransferred       | Long                 | &check;      |
| completionDate         | String               | &check;      |
| createdBy              | RecoveryPointCreator | &check;      |
| creationDate           | String               | &check;      |
| expectedCompletionDate | String               | &check;      |
| iamRoleArn             | String               | &cross;      |
| id                     | String               | &cross;      |
| percentDone            | String               | &check;      |
| recoveryPointArn       | String               | &cross;      |
| region                 | String               | &cross;      |
| resourceArn            | String               | &cross;      |
| resourceType           | String               | &cross;      |
| startBy                | String               | &check;      |
| state                  | String               | &cross;      |
| statusMessage          | String               | &check;      |

#### RecoveryPointCreator
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| backupPlanArn     | String   | &cross;      |
| backupPlanId      | String   | &cross;      |
| backupPlanVersion | String   | &cross;      |
| backupRuleId      | String   | &cross;      |
