---
description: Azure Active Directory App Management Policy
---
azure_ad_app_management_policy
------------------------------

| **Name**     | **Type**                   | **Nullable** |
| ------------ | -------------------------- | ------------ |
| appliesTo    | List<DirectoryObject>      | &check;      |
| description  | String                     | &check;      |
| displayName  | String                     | &check;      |
| id           | String                     | &cross;      |
| isEnabled    | Boolean                    | &check;      |
| oDataType    | String                     | &check;      |
| restrictions | AppManagementConfiguration | &check;      |

#### AppManagementConfiguration
| **Name**            | **Type**                      | **Nullable** |
| ------------------- | ----------------------------- | ------------ |
| keyCredentials      | List<CredentialConfiguration> | &check;      |
| oDataType           | String                        | &check;      |
| passwordCredentials | List<CredentialConfiguration> | &check;      |

#### CredentialConfiguration
| **Name**                            | **Type** | **Nullable** |
| ----------------------------------- | -------- | ------------ |
| maxLifetime                         | String   | &check;      |
| restrictForAppsCreatedAfterDateTime | String   | &check;      |
| restrictionType                     | String   | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |
