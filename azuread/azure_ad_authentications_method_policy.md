---
description: Azure Active Directory Authentications Method Policy
---
azure_ad_authentications_method_policy
--------------------------------------

| **Name**                           | **Type**                                | **Nullable** |
| ---------------------------------- | --------------------------------------- | ------------ |
| authenticationMethodConfigurations | List<AuthenticationMethodConfiguration> | &check;      |
| description                        | String                                  | &check;      |
| displayName                        | String                                  | &check;      |
| id                                 | String                                  | &cross;      |
| lastModifiedDateTime               | String                                  | &check;      |
| oDataType                          | String                                  | &check;      |
| policyMigrationState               | String                                  | &check;      |
| policyVersion                      | String                                  | &check;      |
| reconfirmationInDays               | Int                                     | &check;      |
| registrationEnforcement            | RegistrationEnforcement                 | &check;      |

#### AuthenticationMethodConfiguration
| **Name**       | **Type**            | **Nullable** |
| -------------- | ------------------- | ------------ |
| excludeTargets | List<ExcludeTarget> | &check;      |
| id             | String              | &check;      |
| oDataType      | String              | &check;      |
| state          | String              | &check;      |

#### AuthenticationMethodsRegistrationCampaign
| **Name**             | **Type**            | **Nullable** |
| -------------------- | ------------------- | ------------ |
| excludeTargets       | List<ExcludeTarget> | &check;      |
| includeTargets       | List<IncludeTarget> | &check;      |
| oDataType            | String              | &check;      |
| snoozeDurationInDays | Int                 | &check;      |
| state                | String              | &check;      |

#### ExcludeTarget
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| id         | String   | &check;      |
| oDataType  | String   | &check;      |
| targetType | String   | &check;      |

#### IncludeTarget
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| id                           | String   | &check;      |
| oDataType                    | String   | &check;      |
| targetType                   | String   | &check;      |
| targetedAuthenticationMethod | String   | &check;      |

#### RegistrationEnforcement
| **Name**                                  | **Type**                                  | **Nullable** |
| ----------------------------------------- | ----------------------------------------- | ------------ |
| authenticationMethodsRegistrationCampaign | AuthenticationMethodsRegistrationCampaign | &check;      |
| oDataType                                 | String                                    | &check;      |
