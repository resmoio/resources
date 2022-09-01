---
description: Entity Domain
---
domain
------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| abuseContactEmail | String       | &check;      |
| autoRenew         | Boolean      | &check;      |
| contactEmails     | List<String> | &check;      |
| data              | JSON         | &check;      |
| id                | String       | &cross;      |
| locked            | Boolean      | &check;      |
| name              | String       | &check;      |
| nameServers       | List<String> | &check;      |
| referencedType    | String       | &cross;      |
| registrar         | String       | &check;      |
| tld               | String       | &check;      |

#### BasicResource
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| data           | JSON     | &check;      |
| referencedType | String   | &cross;      |
