---
description: Azure Active Directory Token Issuance Policy
---
azure_ad_token_issuance_policy
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
