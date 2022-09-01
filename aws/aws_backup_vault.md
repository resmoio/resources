---
description: Amazon Web Services Backup Vault
---
aws_backup_vault
----------------

| **Name**               | **Type**           | **Nullable** |
| ---------------------- | ------------------ | ------------ |
| accessPolicy           | JSON               | &check;      |
| accountId              | String             | &cross;      |
| accountName            | String             | &check;      |
| arn                    | String             | &cross;      |
| creationDate           | String             | &check;      |
| creatorRequestId       | String             | &check;      |
| encryptionKeyArn       | String             | &check;      |
| lockDate               | String             | &check;      |
| locked                 | Boolean            | &check;      |
| maxRetentionDays       | Long               | &check;      |
| minRetentionDays       | Long               | &check;      |
| name                   | String             | &cross;      |
| notification           | Notification       | &check;      |
| numberOfRecoveryPoints | Long               | &cross;      |
| region                 | String             | &cross;      |
| tags                   | Map<String,String> | &cross;      |

#### Notification
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| backupVaultEvents | List<String> | &check;      |
| snsTopicArn       | String       | &cross;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

