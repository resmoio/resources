---
description: Google Workspace Mobile Device
---
gsuite_mobile_device
--------------------

| **Name**                       | **Type**          | **Nullable** |
| ------------------------------ | ----------------- | ------------ |
| adbStatus                      | Boolean           | &check;      |
| applications                   | List<Application> | &check;      |
| basebandVersion                | String            | &check;      |
| bootloaderVersion              | String            | &check;      |
| brand                          | String            | &check;      |
| buildNumber                    | String            | &check;      |
| customerId                     | String            | &cross;      |
| defaultLanguage                | String            | &check;      |
| developerOptionsStatus         | Boolean           | &check;      |
| deviceCompromisedStatus        | String            | &check;      |
| deviceId                       | String            | &cross;      |
| devicePasswordStatus           | String            | &check;      |
| email                          | List<String>      | &check;      |
| encryptionStatus               | String            | &check;      |
| firstSync                      | Date              | &check;      |
| hardware                       | String            | &check;      |
| hardwareId                     | String            | &check;      |
| imei                           | String            | &check;      |
| kernelVersion                  | String            | &check;      |
| lastSync                       | Date              | &check;      |
| managedAccountIsOnOwnerProfile | Boolean           | &check;      |
| manufacturer                   | String            | &check;      |
| meid                           | String            | &check;      |
| model                          | String            | &check;      |
| name                           | List<String>      | &check;      |
| networkOperator                | String            | &check;      |
| os                             | String            | &check;      |
| otherAccountsInfo              | List<String>      | &check;      |
| privilege                      | String            | &check;      |
| releaseVersion                 | String            | &check;      |
| resourceId                     | String            | &check;      |
| securityPatchLevel             | Long              | &check;      |
| serialNumber                   | String            | &check;      |
| status                         | String            | &check;      |
| supportsWorkProfile            | Boolean           | &check;      |
| type                           | String            | &check;      |
| unknownSourcesStatus           | Boolean           | &check;      |
| userAgent                      | String            | &check;      |
| wifiMacAddress                 | String            | &check;      |

#### Application
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| displayName | String       | &check;      |
| packageName | String       | &check;      |
| permission  | List<String> | &check;      |
| versionCode | Int          | &check;      |
| versionName | String       | &check;      |
