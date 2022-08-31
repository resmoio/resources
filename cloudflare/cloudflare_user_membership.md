---
description: Cloudflare User Membership
---
cloudflare_user_membership
--------------------------

| **Name**    | **Type**        | **Nullable** |
| ----------- | --------------- | ------------ |
| account     | Account         | &check;      |
| id          | String          | &cross;      |
| permissions | Map<String,Map> | &check;      |
| roles       | List<String>    | &check;      |
| status      | String          | &check;      |

#### Account
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| id       | String             | &check;      |
| name     | String             | &check;      |
| settings | Map<String,String> | &check;      |
