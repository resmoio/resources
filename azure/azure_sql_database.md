---
description: Azure Sql Database
---
azure_sql_database
------------------

| **Name**                          | **Type**                  | **Nullable** |
| --------------------------------- | ------------------------- | ------------ |
| autoPauseDelay                    | Int                       | &check;      |
| catalogCollation                  | String                    | &check;      |
| collation                         | String                    | &check;      |
| createMode                        | String                    | &check;      |
| creationDate                      | String                    | &check;      |
| databaseId                        | String                    | &cross;      |
| defaultSecondaryLocation          | String                    | &check;      |
| earliestRestoreDate               | String                    | &check;      |
| edition                           | String                    | &check;      |
| elasticPoolId                     | String                    | &check;      |
| elasticPoolName                   | String                    | &check;      |
| failoverGroupId                   | String                    | &check;      |
| id                                | String                    | &cross;      |
| kind                              | String                    | &check;      |
| location                          | String                    | &cross;      |
| longTermRetentionBackupResourceId | String                    | &check;      |
| managedBy                         | String                    | &check;      |
| name                              | String                    | &cross;      |
| parentId                          | String                    | &check;      |
| readReplicaCount                  | Int                       | &check;      |
| readScale                         | String                    | &check;      |
| recoverableDatabaseId             | String                    | &check;      |
| recoveryServicesRecoveryPointId   | String                    | &check;      |
| requestedServiceObjectiveName     | String                    | &check;      |
| resourceGroupName                 | String                    | &cross;      |
| restorableDroppedDatabaseId       | String                    | &check;      |
| sampleName                        | String                    | &check;      |
| sku                               | String                    | &check;      |
| sourceDatabaseId                  | String                    | &check;      |
| sqlServerName                     | String                    | &check;      |
| status                            | String                    | &check;      |
| subscriptionId                    | String                    | &cross;      |
| tags                              | Map<String,String>        | &check;      |
| transparentDataEncryption         | TransparentDataEncryption | &check;      |
| type                              | String                    | &cross;      |
| zoneRedundant                     | Boolean                   | &check;      |

#### TransparentDataEncryption
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| databaseName  | String   | &check;      |
| sqlServerName | String   | &check;      |
| status        | String   | &check;      |
