---
description: Amazon Web Services ECR Repository
---
aws_ecr_repository
------------------

| **Name**                   | **Type**                   | **Nullable** |
| -------------------------- | -------------------------- | ------------ |
| accountId                  | String                     | &cross;      |
| accountName                | String                     | &check;      |
| createdAt                  | String                     | &check;      |
| encryptionConfiguration    | EncryptionConfiguration    | &check;      |
| imageScanningConfiguration | ImageScanningConfiguration | &check;      |
| imageTagMutability         | String                     | &check;      |
| region                     | String                     | &cross;      |
| registryId                 | String                     | &check;      |
| repositoryArn              | String                     | &cross;      |
| repositoryName             | String                     | &check;      |
| repositoryUri              | String                     | &check;      |

#### EncryptionConfiguration
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| encryptionType | String   | &check;      |
| kmsKey         | String   | &check;      |

#### ImageScanningConfiguration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| scanOnPush | Boolean  | &check;      |
