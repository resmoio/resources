---
description: Snowflake User
---
snowflake_user
--------------

| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| comment                 | String   | &check;      |
| created_on              | String   | &check;      |
| days_to_expiry          | String   | &check;      |
| default_namespace       | String   | &check;      |
| default_role            | String   | &check;      |
| default_secondary_roles | String   | &check;      |
| default_warehouse       | String   | &check;      |
| disabled                | Boolean  | &check;      |
| display_name            | String   | &check;      |
| email                   | String   | &check;      |
| expires_at_time         | String   | &check;      |
| ext_authn_duo           | Boolean  | &check;      |
| ext_authn_uid           | String   | &check;      |
| first_name              | String   | &check;      |
| has_password            | Boolean  | &check;      |
| has_rsa_public_key      | Boolean  | &check;      |
| last_name               | String   | &check;      |
| last_success_login      | String   | &check;      |
| locked_until_time       | String   | &check;      |
| login_name              | String   | &check;      |
| mins_to_bypass_mfa      | String   | &check;      |
| mins_to_unlock          | String   | &check;      |
| must_change_password    | Boolean  | &check;      |
| name                    | String   | &cross;      |
| owner                   | String   | &check;      |
| snowflake_lock          | Boolean  | &check;      |
