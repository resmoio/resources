---
description: Azure Active Directory Role Management Policy
---
azure_ad_role_management_policy
-------------------------------

| **Name**              | **Type**   | **Nullable** |
| --------------------- | ---------- | ------------ |
| description           | String     | &check;      |
| displayName           | String     | &check;      |
| id                    | String     | &cross;      |
| isOrganizationDefault | Boolean    | &check;      |
| lastModifiedBy        | Identity   | &check;      |
| lastModifiedDateTime  | String     | &check;      |
| oDataType             | String     | &check;      |
| rules                 | List<JSON> | &check;      |
| scopeId               | String     | &check;      |
| scopeType             | String     | &check;      |

#### Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |
| oDataType   | String   | &check;      |
