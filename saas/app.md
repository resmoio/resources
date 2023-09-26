---
description: SaaS Discovered App
---
app
---

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| category          | String       | &check;      |
| categoryOwner     | Owner        | &check;      |
| discoveredOn      | String       | &check;      |
| displayName       | String       | &check;      |
| domains           | List<String> | &check;      |
| isIdentified      | Boolean      | &cross;      |
| issues            | Issues       | &cross;      |
| licence           | Licence      | &check;      |
| name              | String       | &check;      |
| owner             | Owner        | &check;      |
| resmoIntegrations | List<String> | &check;      |
| risk              | RiskScore    | &cross;      |
| securityScore     | Int          | &cross;      |
| status            | String       | &cross;      |
| statusReason      | String       | &check;      |

#### Issues
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| critical | Int      | &cross;      |
| high     | Int      | &cross;      |
| low      | Int      | &cross;      |
| medium   | Int      | &cross;      |
| total    | Int      | &cross;      |

#### Licence
| **Name**    | **Type**      | **Nullable** |
| ----------- | ------------- | ------------ |
| notes       | String        | &check;      |
| period      | String        | &check;      |
| price       | Licence.Price | &check;      |
| renewalDate | Timestamp     | &check;      |

#### Licence.Price
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| amount   | Double   | &cross;      |
| currency | String   | &cross;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| name     | String   | &check;      |

#### RiskScore
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| distributedScore | Double   | &cross;      |
| rawScore         | Double   | &cross;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
