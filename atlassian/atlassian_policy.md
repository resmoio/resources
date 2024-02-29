---
description: Atlassian Policy
---
atlassian_policy
----------------

| **Name**       | **Type**         | **Nullable** |
| -------------- | ---------------- | ------------ |
| attributes     | PolicyAttributes | &check;      |
| id             | String           | &cross;      |
| organizationId | String           | &cross;      |

#### PolicyAttributes
| **Name**  | **Type**             | **Nullable** |
| --------- | -------------------- | ------------ |
| name      | String               | &check;      |
| resources | List<PolicyResource> | &check;      |
| rule      | JSON                 | &check;      |
| status    | String               | &check;      |
| type      | String               | &check;      |

#### PolicyResource
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| applicationStatus | String   | &check;      |
| id                | String   | &check;      |
