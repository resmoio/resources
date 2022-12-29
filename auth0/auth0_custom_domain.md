---
description: Auth0 Custom Domain
---
auth0_custom_domain
-------------------

| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| custom_client_ip_header | String       | &check;      |
| custom_domain_id        | String       | &cross;      |
| domain                  | String       | &check;      |
| origin_domain_name      | String       | &check;      |
| primary                 | Boolean      | &check;      |
| status                  | String       | &check;      |
| tls_policy              | String       | &check;      |
| type                    | String       | &check;      |
| verification            | Verification | &check;      |

#### Verification
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| methods  | List<String> | &check;      |
