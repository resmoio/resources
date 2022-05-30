---
description: Cloudflare Account Member
---
cloudflare_account_members
--------------------------

| **Name**                          | **Type**    | **Nullable** |
| --------------------------------- | ----------- | ------------ |
| account_id                        | String      | &cross;      |
| email                             | String      | &check;      |
| first_name                        | String      | &check;      |
| id                                | String      | &cross;      |
| last_name                         | String      | &check;      |
| roles                             | List<Roles> | &check;      |
| status                            | String      | &check;      |
| two_factor_authentication_enabled | Boolean     | &check;      |

#### Roles
| **Name**    | **Type**        | **Nullable** |
| ----------- | --------------- | ------------ |
| description | String          | &check;      |
| id          | String          | &cross;      |
| name        | String          | &check;      |
| permission  | Map<String,Map> | &check;      |
