---
description: Duo User
---
duo_user
--------

| **Name**            | **Type**                 | **Nullable** |
| ------------------- | ------------------------ | ------------ |
| aliases             | Map<String,String>       | &check;      |
| created             | String                   | &check;      |
| email               | String                   | &check;      |
| firstname           | String                   | &check;      |
| groups              | List<Group>              | &check;      |
| is_enrolled         | Boolean                  | &check;      |
| last_directory_sync | String                   | &check;      |
| last_login          | String                   | &check;      |
| lastname            | String                   | &check;      |
| notes               | String                   | &check;      |
| phones              | List<Phone>              | &check;      |
| realname            | String                   | &check;      |
| status              | String                   | &check;      |
| tokens              | List<MFAToken>           | &check;      |
| user_id             | String                   | &cross;      |
| username            | String                   | &check;      |
| webauthncredentials | List<WebAuthnCredential> | &check;      |

#### Group
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| desc               | String   | &check;      |
| group_id           | String   | &check;      |
| mobile_otp_enabled | Boolean  | &check;      |
| name               | String   | &check;      |
| push_enabled       | Boolean  | &check;      |
| sms_enabled        | Boolean  | &check;      |
| status             | String   | &check;      |
| voice_enabled      | Boolean  | &check;      |

#### MFAToken
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| serial    | String   | &check;      |
| token_id  | String   | &check;      |
| totp_step | String   | &check;      |
| type      | String   | &check;      |

#### Phone
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
| phone_id           | String       | &check;      |
| platform           | String       | &check;      |
| postdelay          | String       | &check;      |
| predelay           | String       | &check;      |
| screenlock         | String       | &check;      |
| sms_passcodes_sent | Boolean      | &check;      |
| tampered           | String       | &check;      |
| type               | String       | &check;      |

#### WebAuthnCredential
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| credential_name | String   | &check;      |
| date_added      | Long     | &check;      |
| label           | String   | &check;      |
| webauthnkey     | String   | &check;      |
