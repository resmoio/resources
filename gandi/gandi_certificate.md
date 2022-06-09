---
description: Gandi Certificate
---
gandi_certificate
-----------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| altnames           | List<String>       | &check;      |
| altnames_unicode   | List<String>       | &check;      |
| assumed_name       | String             | &check;      |
| business_category  | String             | &check;      |
| card_pay_trustlogo | Boolean            | &check;      |
| cert               | String             | &check;      |
| cn                 | String             | &check;      |
| cn_unicode         | String             | &check;      |
| contact            | Contact            | &check;      |
| csr                | String             | &check;      |
| dates              | Dates              | &check;      |
| dcv_method         | String             | &check;      |
| id                 | String             | &cross;      |
| intermediate       | String             | &check;      |
| owner              | String             | &check;      |
| pckg               | CertificatePackage | &check;      |
| reissuable         | Boolean            | &check;      |
| renewable          | Boolean            | &check;      |
| sha_version        | Int                | &check;      |
| sharing_id         | String             | &check;      |
| software           | Int                | &check;      |
| state              | String             | &check;      |
| state_detail       | String             | &check;      |
| status             | String             | &check;      |
| stored             | Boolean            | &check;      |
| trustlogo          | Boolean            | &check;      |

#### CertificatePackage
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| href        | String   | &check;      |
| max_domains | Int      | &check;      |
| name        | String   | &check;      |
| name_label  | String   | &check;      |
| type        | String   | &check;      |
| type_label  | String   | &check;      |
| wildcard    | Boolean  | &check;      |

#### Contact
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| family   | String   | &check;      |
| given    | String   | &check;      |
| orgname  | String   | &check;      |

#### Dates
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| created_at           | String   | &check;      |
| ends_at              | String   | &check;      |
| started_at           | String   | &check;      |
| subscription_ends_at | String   | &check;      |
| updated_at           | String   | &check;      |
