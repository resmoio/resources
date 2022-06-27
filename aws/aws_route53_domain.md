---
description: Amazon Web Services Route53 Domain
---
aws_route53_domain
------------------

| **Name**          | **Type**         | **Nullable** |
| ----------------- | ---------------- | ------------ |
| abuseContactEmail | String           | &check;      |
| abuseContactPhone | String           | &check;      |
| accountId         | String           | &cross;      |
| adminContact      | ContactDetail    | &check;      |
| adminPrivacy      | Boolean          | &check;      |
| autoRenew         | Boolean          | &check;      |
| creationDate      | String           | &check;      |
| dnsSec            | String           | &check;      |
| expirationDate    | String           | &check;      |
| name              | String           | &cross;      |
| nameservers       | List<Nameserver> | &check;      |
| registrantContact | ContactDetail    | &check;      |
| registrantPrivacy | Boolean          | &check;      |
| registrarName     | String           | &check;      |
| registrarUrl      | String           | &check;      |
| registryDomainId  | String           | &check;      |
| reseller          | String           | &check;      |
| statusList        | List<String>     | &check;      |
| techContact       | ContactDetail    | &check;      |
| techPrivacy       | Boolean          | &check;      |
| updatedDate       | String           | &check;      |
| whoIsServer       | String           | &check;      |

#### ContactDetail
| **Name**         | **Type**           | **Nullable** |
| ---------------- | ------------------ | ------------ |
| addressLine1     | String             | &check;      |
| addressLine2     | String             | &check;      |
| city             | String             | &check;      |
| contactType      | String             | &check;      |
| countryCode      | String             | &check;      |
| email            | String             | &check;      |
| extraParams      | Map<String,String> | &check;      |
| fax              | String             | &check;      |
| firstName        | String             | &check;      |
| lastName         | String             | &check;      |
| organizationName | String             | &check;      |
| phoneNumber      | String             | &check;      |
| state            | String             | &check;      |
| zipCode          | String             | &check;      |

#### Nameserver
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| glueIps  | List<String> | &check;      |
| name     | String       | &check;      |
