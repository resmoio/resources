---
description: Duo Account
---
duo_account
-----------

| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| caller_id                      | String   | &check;      |
| fraud_email                    | String   | &check;      |
| fraud_email_enabled            | Boolean  | &check;      |
| helpdesk_bypass                | String   | &check;      |
| helpdesk_bypass_expiration     | Int      | &check;      |
| helpdesk_can_send_enroll_email | Boolean  | &check;      |
| helpdesk_message               | String   | &check;      |
| inactive_user_expiration       | Int      | &check;      |
| keypress_confirm               | String   | &check;      |
| keypress_fraud                 | String   | &check;      |
| language                       | String   | &check;      |
| lockout_expire_duration        | Int      | &check;      |
| lockout_threshold              | Int      | &check;      |
| minimum_password_length        | Int      | &check;      |
| mobile_otp_enabled             | Boolean  | &check;      |
| name                           | String   | &cross;      |
| password_requires_lower_alpha  | Boolean  | &check;      |
| password_requires_numeric      | Boolean  | &check;      |
| password_requires_special      | Boolean  | &check;      |
| password_requires_upper_alpha  | Boolean  | &check;      |
| push_enabled                   | Boolean  | &check;      |
| sms_batch                      | Int      | &check;      |
| sms_enabled                    | Boolean  | &check;      |
| sms_expiration                 | Int      | &check;      |
| sms_message                    | String   | &check;      |
| sms_refresh                    | Int      | &check;      |
| telephony_warning_min          | Int      | &check;      |
| timezone                       | String   | &check;      |
| user_telephony_cost_max        | Int      | &check;      |
| voice_enabled                  | Boolean  | &check;      |
