---
description: Amazon Web Services Backup Restore Job
---
aws_backup_restore_job
----------------------

| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| accountId                     | String   | &cross;      |
| accountName                   | String   | &check;      |
| backupSizeInBytes             | Long     | &check;      |
| completionDate                | String   | &check;      |
| createdResourceArn            | String   | &check;      |
| creationDate                  | String   | &check;      |
| expectedCompletionTimeMinutes | Long     | &check;      |
| iamRoleArn                    | String   | &cross;      |
| id                            | String   | &cross;      |
| percentDone                   | String   | &check;      |
| recoveryPointArn              | String   | &cross;      |
| region                        | String   | &cross;      |
| resourceType                  | String   | &cross;      |
| restoreJobAccountId           | String   | &cross;      |
| status                        | String   | &cross;      |
| statusMessage                 | String   | &check;      |
