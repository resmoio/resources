---
description: Azure Storage Blob Container
---
azure_storage_blob_container
----------------------------

| **Name**          | **Type**                    | **Nullable** |
| ----------------- | --------------------------- | ------------ |
| deleted           | Boolean                     | &check;      |
| metadata          | Map<String,String>          | &check;      |
| name              | String                      | &cross;      |
| properties        | BlobContainerItemProperties | &check;      |
| resourceGroupName | String                      | &cross;      |
| storageAccountId  | String                      | &cross;      |
| subscriptionId    | String                      | &cross;      |
| version           | String                      | &check;      |

#### BlobContainerItemProperties
| **Name**                                | **Type** | **Nullable** |
| --------------------------------------- | -------- | ------------ |
| defaultEncryptionScope                  | String   | &check;      |
| deletedTime                             | String   | &check;      |
| encryptionScopeOverridePrevented        | Boolean  | &check;      |
| etag                                    | String   | &check;      |
| hasImmutabilityPolicy                   | Boolean  | &check;      |
| hasLegalHold                            | Boolean  | &check;      |
| isImmutableStorageWithVersioningEnabled | Boolean  | &check;      |
| lastModified                            | String   | &check;      |
| leaseDuration                           | String   | &check;      |
| leaseState                              | String   | &check;      |
| leaseStatus                             | String   | &check;      |
| publicAccess                            | String   | &check;      |
| remainingRetentionDays                  | Int      | &check;      |
