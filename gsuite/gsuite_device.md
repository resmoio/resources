---
description: Google Workspace Device
---
gsuite_device
-------------

| **Name**                  | **Type**                   | **Nullable** |
| ------------------------- | -------------------------- | ------------ |
| androidSpecificAttributes | AndroidAttributes          | &check;      |
| assetTag                  | String                     | &check;      |
| basebandVersion           | String                     | &check;      |
| bootloaderVersion         | String                     | &check;      |
| brand                     | String                     | &check;      |
| buildNumber               | String                     | &check;      |
| certificateAttributes     | List<CertificateAttribute> | &check;      |
| compromisedState          | String                     | &check;      |
| createTime                | String                     | &check;      |
| customerId                | String                     | &cross;      |
| deviceId                  | String                     | &cross;      |
| deviceType                | String                     | &check;      |
| enabledDeveloperOptions   | Boolean                    | &check;      |
| enabledUsbDebugging       | Boolean                    | &check;      |
| encryptionState           | String                     | &check;      |
| imei                      | String                     | &check;      |
| kernelVersion             | String                     | &check;      |
| lastSyncTime              | String                     | &check;      |
| managementState           | String                     | &check;      |
| manufacturer              | String                     | &check;      |
| meid                      | String                     | &check;      |
| model                     | String                     | &check;      |
| name                      | String                     | &check;      |
| networkOperator           | String                     | &check;      |
| osVersion                 | String                     | &check;      |
| otherAccounts             | List<String>               | &check;      |
| ownerType                 | String                     | &check;      |
| releaseVersion            | String                     | &check;      |
| securityPatchTime         | String                     | &check;      |
| serialNumber              | String                     | &check;      |
| users                     | List<User>                 | &cross;      |
| wifiMacAddresses          | List<String>               | &check;      |

#### AndroidAttributes
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| enabledUnknownSources | Boolean  | &check;      |
| ownerProfileAccount   | Boolean  | &check;      |
| ownershipPrivilege    | String   | &check;      |
| supportsWorkProfile   | Boolean  | &check;      |

#### CertificateAttribute
| **Name**               | **Type**            | **Nullable** |
| ---------------------- | ------------------- | ------------ |
| certificateTemplate    | CertificateTemplate | &check;      |
| fingerprint            | String              | &check;      |
| issuer                 | String              | &check;      |
| serialNumber           | String              | &check;      |
| subject                | String              | &check;      |
| thumbprint             | String              | &check;      |
| validationState        | String              | &check;      |
| validityExpirationTime | String              | &check;      |
| validityStartTime      | String              | &check;      |

#### CertificateTemplate
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| id           | String   | &check;      |
| majorVersion | Int      | &check;      |
| minorVersion | Int      | &check;      |

#### User
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| compromisedState | String   | &check;      |
| createTime       | String   | &check;      |
| firstSyncTime    | String   | &check;      |
| languageCode     | String   | &check;      |
| lastSyncTime     | String   | &check;      |
| managementState  | String   | &check;      |
| name             | String   | &check;      |
| passwordState    | String   | &check;      |
| userAgent        | String   | &check;      |
| userEmail        | String   | &check;      |
