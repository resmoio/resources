---
description: Google Cloud Platform KMS Crypto Key
---
gcp_kms_crypto_key
------------------

| **Name**                 | **Type**                 | **Nullable** |
| ------------------------ | ------------------------ | ------------ |
| createTime               | String                   | &check;      |
| destroyScheduledDuration | String                   | &check;      |
| importOnly               | Boolean                  | &check;      |
| keyRing                  | String                   | &cross;      |
| labels                   | Map<String,String>       | &check;      |
| name                     | String                   | &cross;      |
| nextRotationTime         | String                   | &check;      |
| primary                  | CryptoKeyVersion         | &check;      |
| project                  | String                   | &cross;      |
| purpose                  | String                   | &check;      |
| rotationPeriod           | String                   | &check;      |
| versionTemplate          | CryptoKeyVersionTemplate | &check;      |

#### CryptoKeyVersion
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| algorithm           | String   | &check;      |
| createTime          | String   | &check;      |
| destroyEventTime    | String   | &check;      |
| destroyTime         | String   | &check;      |
| generateTime        | String   | &check;      |
| importFailureReason | String   | &check;      |
| importJob           | String   | &check;      |
| importTime          | String   | &check;      |
| name                | String   | &check;      |
| protectionLevel     | String   | &check;      |
| reimportEligible    | Boolean  | &check;      |
| state               | String   | &check;      |

#### CryptoKeyVersionTemplate
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| algorithm       | String   | &check;      |
| protectionLevel | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
