---
description: SaaS User
---
user
----

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| alternativeEmails | List<String> | &check;      |
| apps              | List<String> | &cross;      |
| createdDate       | String       | &cross;      |
| deletedDate       | String       | &check;      |
| devices           | Int          | &cross;      |
| email             | String       | &cross;      |
| isActive          | Boolean      | &cross;      |
| isMonitored       | Boolean      | &cross;      |
| issues            | Issues       | &cross;      |
| name              | String       | &cross;      |
| offBoardDate      | String       | &check;      |
| phoneNumber       | String       | &check;      |
| riskScore         | Double       | &cross;      |
| slackHandle       | String       | &check;      |
| teams             | List<Team>   | &cross;      |

#### Issues
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| critical | Int      | &cross;      |
| high     | Int      | &cross;      |
| low      | Int      | &cross;      |
| medium   | Int      | &cross;      |
| total    | Int      | &cross;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
