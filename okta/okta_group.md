---
description: Okta Group
---
okta_group
----------

| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| created               | String       | &check;      |
| groupRoleIds          | List<String> | &check;      |
| id                    | String       | &cross;      |
| lastMembershipUpdated | String       | &check;      |
| lastUpdated           | String       | &check;      |
| profile               | Profile      | &check;      |
| type                  | String       | &check;      |

#### Profile
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| name        | String   | &check;      |
