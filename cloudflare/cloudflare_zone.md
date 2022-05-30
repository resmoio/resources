---
description: Cloudflare Zone
---
cloudflare_zone
---------------

| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| account               | Account      | &cross;      |
| activated_on          | String       | &check;      |
| created_on            | String       | &check;      |
| id                    | String       | &cross;      |
| meta                  | Meta         | &check;      |
| name                  | String       | &check;      |
| name_servers          | List<String> | &check;      |
| original_dnshost      | String       | &check;      |
| original_name_servers | List<String> | &check;      |
| original_registrar    | String       | &check;      |
| owner                 | Owner        | &check;      |
| paused                | Boolean      | &cross;      |
| permissions           | List<String> | &check;      |
| status                | String       | &check;      |
| type                  | String       | &check;      |

#### Account
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |

#### Meta
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| custom_certificate_quota  | Number   | &check;      |
| multiple_railguns_allowed | Boolean  | &check;      |
| page_rule_quota           | Number   | &check;      |
| phishing_detected         | Boolean  | &check;      |
| step                      | Number   | &check;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |
| type     | String   | &check;      |
