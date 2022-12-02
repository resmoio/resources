---
description: Vercel Domain
---
vercel_domain
-------------

| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| boughtAt            | Long         | &check;      |
| createdAt           | Long         | &check;      |
| creator             | Creator      | &check;      |
| customNameservers   | List<String> | &check;      |
| expiresAt           | Long         | &check;      |
| id                  | String       | &cross;      |
| intendedNameservers | List<String> | &check;      |
| name                | String       | &check;      |
| nameservers         | List<String> | &check;      |
| orderedAt           | Long         | &check;      |
| projectId           | String       | &check;      |
| renew               | Boolean      | &check;      |
| serviceType         | String       | &check;      |
| transferStartedAt   | Long         | &check;      |
| transferredAt       | Long         | &check;      |
| verified            | Boolean      | &check;      |

#### Creator
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| customerId       | String   | &check;      |
| email            | String   | &check;      |
| id               | String   | &check;      |
| isDomainReseller | Boolean  | &check;      |
| username         | String   | &check;      |
