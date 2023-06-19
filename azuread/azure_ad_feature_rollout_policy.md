---
description: Azure Active Directory Feature Rollout Policy
---
azure_ad_feature_rollout_policy
-------------------------------

| **Name**                | **Type**              | **Nullable** |
| ----------------------- | --------------------- | ------------ |
| appliesTo               | List<DirectoryObject> | &check;      |
| description             | String                | &check;      |
| displayName             | String                | &check;      |
| feature                 | String                | &check;      |
| id                      | String                | &cross;      |
| isAppliedToOrganization | Boolean               | &check;      |
| isEnabled               | Boolean               | &check;      |
| oDataType               | String                | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |
