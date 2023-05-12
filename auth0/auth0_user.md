---
description: Auth0 User
---
auth0_user
----------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| app_metadata   | JSON           | &check;      |
| blocked        | Boolean        | &check;      |
| created_at     | String         | &check;      |
| email          | String         | &check;      |
| email_verified | Boolean        | &check;      |
| family_name    | String         | &check;      |
| given_name     | String         | &check;      |
| identities     | List<Identity> | &check;      |
| last_ip        | String         | &check;      |
| last_login     | String         | &check;      |
| logins_count   | Int            | &check;      |
| multifactor    | List<String>   | &check;      |
| name           | String         | &check;      |
| nickname       | String         | &check;      |
| phone_number   | String         | &check;      |
| phone_verified | Boolean        | &check;      |
| updated_at     | String         | &check;      |
| user_id        | String         | &cross;      |
| user_metadata  | JSON           | &check;      |
| username       | String         | &check;      |

#### Identity
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| connection | String   | &check;      |
| isSocial   | Boolean  | &check;      |
| provider   | String   | &check;      |
| user_id    | String   | &check;      |
