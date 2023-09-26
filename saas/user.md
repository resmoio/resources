---
description: SaaS User
---
user
----

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| alternativeEmails | List<String> | &check;      |
| createdDate       | String       | &cross;      |
| deactivatedDate   | String       | &check;      |
| deletedDate       | String       | &check;      |
| devices           | Int          | &cross;      |
| email             | String       | &cross;      |
| issues            | Issues       | &cross;      |
| name              | String       | &cross;      |
| phoneNumber       | String       | &check;      |
| risk              | RiskScore    | &cross;      |
| slackHandle       | SlackHandle  | &check;      |
| status            | String       | &check;      |
| teams             | List<Team>   | &cross;      |

#### Issues
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| critical | Int      | &cross;      |
| high     | Int      | &cross;      |
| low      | Int      | &cross;      |
| medium   | Int      | &cross;      |
| total    | Int      | &cross;      |

#### RiskScore
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| distributedScore | Double   | &cross;      |
| rawScore         | Double   | &cross;      |

#### SlackHandle
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| url      | String   | &cross;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
