---
description: Azure Active Directory Device
---
azure_ad_device
---------------

| **Name**                      | **Type**                    | **Nullable** |
| ----------------------------- | --------------------------- | ------------ |
| accountEnabled                | Boolean                     | &check;      |
| alternativeSecurityIds        | List<AlternativeSecurityId> | &check;      |
| approximateLastSignInDateTime | String                      | &check;      |
| complianceExpirationDateTime  | String                      | &check;      |
| deviceCategory                | String                      | &check;      |
| deviceId                      | String                      | &check;      |
| deviceMetadata                | String                      | &check;      |
| deviceOwnership               | String                      | &check;      |
| deviceVersion                 | Int                         | &check;      |
| displayName                   | String                      | &check;      |
| enrollmentProfileName         | String                      | &check;      |
| id                            | String                      | &cross;      |
| isCompliant                   | Boolean                     | &check;      |
| isManaged                     | Boolean                     | &check;      |
| mdmAppId                      | String                      | &check;      |
| memberOf                      | List<DirectoryObject>       | &check;      |
| oDataType                     | String                      | &check;      |
| onPremisesLastSyncDateTime    | String                      | &check;      |
| onPremisesSyncEnabled         | Boolean                     | &check;      |
| operatingSystem               | String                      | &check;      |
| operatingSystemVersion        | String                      | &check;      |
| physicalIds                   | List<String>                | &check;      |
| profileType                   | String                      | &check;      |
| registeredOwners              | List<DirectoryObject>       | &check;      |
| registeredUsers               | List<DirectoryObject>       | &check;      |
| registrationDateTime          | String                      | &check;      |
| systemLabels                  | List<String>                | &check;      |
| transitiveMemberOf            | List<DirectoryObject>       | &check;      |
| trustType                     | String                      | &check;      |

#### AlternativeSecurityId
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| identityProvider | String   | &check;      |
| oDataType        | String   | &check;      |
| type             | Int      | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |
