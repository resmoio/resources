---
description: Duo MFA Token
---
duo_mfa_token
-------------

| **Name**  | **Type**    | **Nullable** |
| --------- | ----------- | ------------ |
| admins    | List<Admin> | &check;      |
| serial    | String      | &check;      |
| token_id  | String      | &cross;      |
| totp_step | String      | &check;      |
| type      | String      | &check;      |
| users     | List<User>  | &check;      |

#### Admin
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| admin_id | String   | &check;      |
| email    | String   | &check;      |
| name     | String   | &check;      |
| role     | String   | &check;      |
| status   | String   | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| status   | String   | &check;      |
| user_id  | String   | &check;      |
| username | String   | &check;      |
