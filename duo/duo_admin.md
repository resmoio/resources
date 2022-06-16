---
description: Duo Admin
---
duo_admin
---------

| **Name**                  | **Type**      | **Nullable** |
| ------------------------- | ------------- | ------------ |
| admin_id                  | String        | &cross;      |
| admin_units               | List<String>  | &check;      |
| created                   | String        | &check;      |
| email                     | String        | &check;      |
| hardtoken                 | HardwareToken | &check;      |
| last_login                | String        | &check;      |
| name                      | String        | &check;      |
| password_change_required  | Boolean       | &check;      |
| phone                     | String        | &check;      |
| restricted_by_admin_units | Boolean       | &check;      |
| role                      | String        | &check;      |
| status                    | String        | &check;      |

#### HardwareToken
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| serial    | String   | &check;      |
| token_id  | String   | &check;      |
| totp_step | String   | &check;      |
| type      | String   | &check;      |
