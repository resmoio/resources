---
description: Amazon Web Services DynamoDB Backup
---
aws_dynamodb_backup
-------------------

| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| accountId              | String   | &cross;      |
| backupArn              | String   | &cross;      |
| backupCreationDateTime | String   | &check;      |
| backupExpiryDateTime   | String   | &check;      |
| backupName             | String   | &check;      |
| backupSizeBytes        | Long     | &check;      |
| backupStatus           | String   | &check;      |
| backupType             | String   | &check;      |
| region                 | String   | &cross;      |
| tableArn               | String   | &check;      |
| tableId                | String   | &check;      |
| tableName              | String   | &check;      |
