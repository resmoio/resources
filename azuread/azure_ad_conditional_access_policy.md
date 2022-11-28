---
description: Azure Active Directory Conditional Access Policy
---
azure_ad_conditional_access_policy
----------------------------------

| **Name**        | **Type**        | **Nullable** |
| --------------- | --------------- | ------------ |
| conditions      | Conditions      | &check;      |
| createdDateTime | String          | &check;      |
| description     | String          | &check;      |
| displayName     | String          | &check;      |
| grantControls   | GrantControls   | &check;      |
| id              | String          | &cross;      |
| oDataType       | String          | &check;      |
| sessionControls | SessionControls | &check;      |
| state           | String          | &check;      |

#### Applications
| **Name**                                    | **Type**     | **Nullable** |
| ------------------------------------------- | ------------ | ------------ |
| excludeApplications                         | List<String> | &check;      |
| includeApplications                         | List<String> | &check;      |
| includeAuthenticationContextClassReferences | List<String> | &check;      |
| includeUserActions                          | List<String> | &check;      |
| oDataType                                   | String       | &check;      |

#### ClientApplications
| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| excludeServicePrincipals | List<String> | &check;      |
| includeServicePrincipals | List<String> | &check;      |
| oDataType                | String       | &check;      |

#### Conditions
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| applications       | Applications       | &check;      |
| clientAppTypes     | List<String>       | &check;      |
| clientApplications | ClientApplications | &check;      |
| deviceFilters      | DeviceFilter       | &check;      |
| locations          | Locations          | &check;      |
| oDataType          | String             | &check;      |
| platforms          | Platforms          | &check;      |
| signInRiskLevels   | List<String>       | &check;      |
| users              | Users              | &check;      |

#### DeviceFilter
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| filterMode | String   | &check;      |
| oDataType  | String   | &check;      |
| rule       | String   | &check;      |

#### GrantControls
| **Name**                    | **Type**     | **Nullable** |
| --------------------------- | ------------ | ------------ |
| builtInControls             | List<String> | &check;      |
| customAuthenticationFactors | List<String> | &check;      |
| oDataType                   | String       | &check;      |
| operator                    | String       | &check;      |
| termsOfUse                  | List<String> | &check;      |

#### Locations
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| excludeLocations | List<String> | &check;      |
| includeLocations | List<String> | &check;      |
| oDataType        | String       | &check;      |

#### Platforms
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| excludePlatforms | List<String> | &check;      |
| includePlatforms | List<String> | &check;      |
| oDataType        | String       | &check;      |

#### SessionControls
| **Name**                               | **Type** | **Nullable** |
| -------------------------------------- | -------- | ------------ |
| applicationEnforcedRestrictionsEnabled | Boolean  | &check;      |
| cloudAppSecurityEnabled                | Boolean  | &check;      |
| disableResilienceDefaults              | Boolean  | &check;      |
| oDataType                              | String   | &check;      |
| persistentBrowserMode                  | String   | &check;      |
| signInFrequencyType                    | String   | &check;      |
| signInFrequencyValue                   | Int      | &check;      |

#### Users
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| excludeGroups | List<String> | &check;      |
| excludeRoles  | List<String> | &check;      |
| excludeUsers  | List<String> | &check;      |
| includeGroups | List<String> | &check;      |
| includeRoles  | List<String> | &check;      |
| includeUsers  | List<String> | &check;      |
| oDataType     | String       | &check;      |
