---
description: Azure Active Directory Tenant App Management Policy
---
azure_ad_tenant_app_management_policy
-------------------------------------

| **Name**                     | **Type**                   | **Nullable** |
| ---------------------------- | -------------------------- | ------------ |
| applicationRestrictions      | AppManagementConfiguration | &check;      |
| description                  | String                     | &check;      |
| displayName                  | String                     | &check;      |
| id                           | String                     | &cross;      |
| isEnabled                    | Boolean                    | &check;      |
| oDataType                    | String                     | &check;      |
| servicePrincipalRestrictions | AppManagementConfiguration | &check;      |

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
