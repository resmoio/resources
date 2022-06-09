---
description: Gandi Domain Contact
---
gandi_domain_contact
--------------------

| **Name**   | **Type**      | **Nullable** |
| ---------- | ------------- | ------------ |
| admin      | ContactDetail | &check;      |
| bill       | ContactDetail | &check;      |
| domainfqdn | String        | &cross;      |
| owner      | ContactDetail | &check;      |
| tech       | ContactDetail | &check;      |

#### ContactDetail
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| city             | String   | &check;      |
| country          | String   | &check;      |
| data_obfuscated  | Boolean  | &check;      |
| email            | String   | &check;      |
| extra_parameters | JSON     | &check;      |
| family           | String   | &check;      |
| given            | String   | &check;      |
| mail_obfuscated  | Boolean  | &check;      |
| orgname          | String   | &check;      |
| phone            | String   | &check;      |
| same_as_owner    | Boolean  | &check;      |
| state            | String   | &check;      |
| streetaddr       | String   | &check;      |
| type             | Int      | &check;      |
| zip              | String   | &check;      |
