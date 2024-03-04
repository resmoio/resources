---
description: Okta Trusted Origin
---
okta_trusted_origin
-------------------

| **Name**      | **Type**    | **Nullable** |
| ------------- | ----------- | ------------ |
| created       | String      | &check;      |
| createdBy     | String      | &check;      |
| id            | String      | &cross;      |
| lastUpdated   | String      | &check;      |
| lastUpdatedBy | String      | &check;      |
| name          | String      | &check;      |
| origin        | String      | &check;      |
| scopes        | List<Scope> | &check;      |
| status        | String      | &check;      |

#### Scope
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| allowedOktaApps | List<String> | &check;      |
| type            | String       | &check;      |
