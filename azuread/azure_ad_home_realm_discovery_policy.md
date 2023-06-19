---
description: Azure Active Directory Home Realm Discovery Policy
---
azure_ad_home_realm_discovery_policy
------------------------------------

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
