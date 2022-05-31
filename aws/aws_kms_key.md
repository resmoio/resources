---
description: Amazon Web Services KMS Key
---
aws_kms_key
-----------

| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| accountId       | String             | &cross;      |
| arn             | String             | &cross;      |
| id              | String             | &cross;      |
| metadata        | Metadata           | &check;      |
| policy          | List<Policy>       | &cross;      |
| region          | String             | &cross;      |
| rotationEnabled | Boolean            | &check;      |
| tags            | Map<String,String> | &cross;      |

#### Metadata
| **Name**                    | **Type**     | **Nullable** |
| --------------------------- | ------------ | ------------ |
| cloudHsmClusterId           | String       | &check;      |
| creationDate                | String       | &check;      |
| customKeyStoreId            | String       | &check;      |
| deletionDate                | String       | &check;      |
| description                 | String       | &check;      |
| enabled                     | Boolean      | &check;      |
| encryptionAlgorithms        | List<String> | &check;      |
| expirationModel             | String       | &check;      |
| keyManager                  | String       | &check;      |
| keySpec                     | String       | &check;      |
| keyUsage                    | String       | &check;      |
| multiRegion                 | Boolean      | &cross;      |
| multiRegionKeyType          | String       | &check;      |
| pendingDeletionWindowInDays | Int          | &check;      |
| signingAlgorithms           | List<String> | &check;      |
| validTo                     | String       | &check;      |

#### Policy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| content  | JSON     | &check;      |
| name     | String   | &cross;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

