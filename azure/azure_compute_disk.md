---
description: Azure Compute Disk
---
azure_compute_disk
------------------

| **Name**                   | **Type**            | **Nullable** |
| -------------------------- | ------------------- | ------------ |
| acceleratedNetwork         | Boolean             | &check;      |
| architecture               | String              | &check;      |
| availabilityZones          | List<String>        | &check;      |
| burstingEnabled            | Boolean             | &check;      |
| creationData               | CreationData        | &check;      |
| creationMethod             | String              | &check;      |
| dataAccessAuthMode         | String              | &check;      |
| diskAccessId               | String              | &check;      |
| diskIopsReadOnly           | Long                | &check;      |
| diskIopsReadWrite          | Long                | &check;      |
| diskMBpsReadOnly           | Long                | &check;      |
| diskMBpsReadWrite          | Long                | &check;      |
| diskState                  | String              | &check;      |
| encryption                 | Encryption          | &check;      |
| encryptionEnabled          | Boolean             | &check;      |
| extendedLocation           | ExtendedLocation    | &check;      |
| hyperVGeneration           | String              | &check;      |
| id                         | String              | &cross;      |
| isAttachedToVirtualMachine | Boolean             | &check;      |
| location                   | String              | &cross;      |
| managedBy                  | String              | &check;      |
| managedByExtended          | List<String>        | &check;      |
| maxShares                  | Int                 | &check;      |
| name                       | String              | &cross;      |
| networkAccessPolicy        | String              | &check;      |
| osType                     | String              | &check;      |
| provisioningState          | String              | &check;      |
| publicNetworkAccess        | String              | &check;      |
| purchasePlan               | PurchasePlan        | &check;      |
| resourceGroupName          | String              | &cross;      |
| securityProfile            | DiskSecurityProfile | &check;      |
| shareInfo                  | List<String>        | &check;      |
| sku                        | String              | &check;      |
| source                     | Source              | &check;      |
| subscriptionId             | String              | &cross;      |
| supportsHibernation        | Boolean             | &check;      |
| tags                       | Map<String,String>  | &check;      |
| tier                       | String              | &check;      |
| timeCreated                | String              | &check;      |
| type                       | String              | &cross;      |
| uniqueId                   | String              | &check;      |
| virtualMachineId           | String              | &check;      |
| zones                      | List<String>        | &check;      |

#### CreationData
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| createOption            | String   | &check;      |
| galleryImageReferenceId | String   | &check;      |
| imageReferenceId        | String   | &check;      |
| logicalSectorSize       | Int      | &check;      |
| securityDataUri         | String   | &check;      |
| sourceResourceId        | String   | &check;      |
| sourceUniqueId          | String   | &check;      |
| sourceUri               | String   | &check;      |
| storageAccountId        | String   | &check;      |
| uploadSizeBytes         | Long     | &check;      |

#### DiskSecurityProfile
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| secureVMDiskEncryptionSetId | String   | &check;      |
| securityType                | String   | &check;      |

#### Encryption
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| diskEncryptionSetId | String   | &check;      |
| type                | String   | &check;      |

#### ExtendedLocation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### PurchasePlan
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| name          | String   | &check;      |
| product       | String   | &check;      |
| promotionCode | String   | &check;      |
| publisher     | String   | &check;      |

#### Source
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| type     | String   | &check;      |
