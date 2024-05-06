---
description: Okta User Grant
---
okta_user_grant
---------------

| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| clientId    | String   | &check;      |
| created     | String   | &check;      |
| createdBy   | User     | &check;      |
| id          | String   | &cross;      |
| issuer      | String   | &check;      |
| lastUpdated | String   | &check;      |
| scopeId     | String   | &check;      |
| source      | String   | &check;      |
| status      | String   | &check;      |
| userId      | String   | &cross;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| type     | String   | &check;      |
