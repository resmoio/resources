---
description: Cloudflare User Account
---
cloudflare_user_account
-----------------------

| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
| settings | Settings | &check;      |
| type     | String   | &check;      |

#### Settings
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| access_approval_expiry           | String   | &check;      |
| enforce_twofactor                | Boolean  | &check;      |
| use_account_custom_ns_by_default | Boolean  | &check;      |
