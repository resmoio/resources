---
description: Duo Phone
---
duo_phone
---------

| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| activated          | Boolean      | &check;      |
| capabilities       | List<String> | &check;      |
| encrypted          | String       | &check;      |
| extension          | String       | &check;      |
| fingerprint        | String       | &check;      |
| last_seen          | String       | &check;      |
| model              | String       | &check;      |
| name               | String       | &check;      |
| number             | String       | &check;      |
| phone_id           | String       | &cross;      |
| platform           | String       | &check;      |
| postdelay          | String       | &check;      |
| predelay           | String       | &check;      |
| screenlock         | String       | &check;      |
| sms_passcodes_sent | Boolean      | &check;      |
| tampered           | String       | &check;      |
| type               | String       | &check;      |
| users              | List<User>   | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| status   | String   | &check;      |
| user_id  | String   | &check;      |
| username | String   | &check;      |
