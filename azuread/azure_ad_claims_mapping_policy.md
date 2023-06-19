---
description: Azure Active Directory Claims Mapping Policy
---
azure_ad_claims_mapping_policy
------------------------------

| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| appliesTo             | List<DirectoryObject> | &check;      |
| definition            | List<String>          | &check;      |
| description           | String                | &check;      |
| displayName           | String                | &check;      |
| id                    | String                | &cross;      |
| isOrganizationDefault | Boolean               | &check;      |
| oDataType             | String                | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |
