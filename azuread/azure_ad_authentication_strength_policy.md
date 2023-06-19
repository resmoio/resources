---
description: Azure Active Directory Authentication Strength Policy
---
azure_ad_authentication_strength_policy
---------------------------------------

| **Name**                  | **Type**                                     | **Nullable** |
| ------------------------- | -------------------------------------------- | ------------ |
| allowedCombinations       | List<List>                                   | &check;      |
| combinationConfigurations | List<AuthenticationCombinationConfiguration> | &check;      |
| createdDateTime           | String                                       | &check;      |
| description               | String                                       | &check;      |
| displayName               | String                                       | &check;      |
| id                        | String                                       | &cross;      |
| modifiedDateTime          | String                                       | &check;      |
| oDataType                 | String                                       | &check;      |
| policyType                | String                                       | &check;      |
| requirementsSatisfied     | List<String>                                 | &check;      |

#### AuthenticationCombinationConfiguration
| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| allowedAAGUIDs        | List<String> | &check;      |
| appliesToCombinations | List<List>   | &check;      |
| id                    | String       | &check;      |
| oDataType             | String       | &check;      |
