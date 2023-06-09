---
description: Atlassian Access Domain
---
atlassian_access_domain
-----------------------

| **Name**       | **Type**         | **Nullable** |
| -------------- | ---------------- | ------------ |
| attributes     | DomainAttributes | &check;      |
| id             | String           | &cross;      |
| organizationId | String           | &cross;      |

#### Claim
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| status   | String   | &check;      |
| type     | String   | &check;      |

#### DomainAttributes
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| claim    | Claim    | &check;      |
| name     | String   | &check;      |
