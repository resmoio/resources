---
description: Okta Domain
---
okta_domain
-----------

| **Name**              | **Type**        | **Nullable** |
| --------------------- | --------------- | ------------ |
| certificateSourceType | String          | &check;      |
| dnsRecords            | List<DnsRecord> | &check;      |
| domain                | String          | &check;      |
| id                    | String          | &cross;      |
| validationStatus      | String          | &check;      |

#### DnsRecord
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| expiration | String       | &check;      |
| fqdn       | String       | &check;      |
| recordType | String       | &check;      |
| values     | List<String> | &check;      |
