---
description: Cloudflare User
---
cloudflare_user
---------------

| **Name**                          | **Type**           | **Nullable** |
| --------------------------------- | ------------------ | ------------ |
| country                           | String             | &check;      |
| created_on                        | String             | &check;      |
| email                             | String             | &check;      |
| first_name                        | String             | &check;      |
| has_business_zones                | Boolean            | &cross;      |
| has_enterprise_zones              | Boolean            | &cross;      |
| has_pro_zones                     | Boolean            | &cross;      |
| id                                | String             | &cross;      |
| last_name                         | String             | &check;      |
| organizations                     | List<Organization> | &check;      |
| suspended                         | Boolean            | &cross;      |
| telephone                         | String             | &check;      |
| two_factor_authentication_enabled | Boolean            | &cross;      |
| two_factor_authentication_locked  | Boolean            | &cross;      |
| username                          | String             | &check;      |
| zipcode                           | String             | &check;      |

#### Organization
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| id          | String       | &cross;      |
| name        | String       | &check;      |
| permissions | List<String> | &check;      |
| roles       | List<String> | &check;      |
| status      | String       | &check;      |
