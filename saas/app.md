---
description: SaaS Discovered App
---
app
---

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| category          | String       | &check;      |
| categoryOwner     | Owner        | &check;      |
| displayName       | String       | &check;      |
| domains           | List<String> | &check;      |
| isIdentified      | Boolean      | &cross;      |
| issues            | Issues       | &cross;      |
| name              | String       | &check;      |
| owner             | Owner        | &check;      |
| resmoIntegrations | List<String> | &check;      |
| riskScore         | Double       | &cross;      |
| securityScore     | Double       | &cross;      |
| status            | String       | &cross;      |

#### Issues
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| critical | Int      | &cross;      |
| high     | Int      | &cross;      |
| low      | Int      | &cross;      |
| medium   | Int      | &cross;      |
| total    | Int      | &cross;      |

#### Owner
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| email        | String   | &check;      |
| isResmoOwner | Boolean  | &cross;      |
| name         | String   | &check;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
