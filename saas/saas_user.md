---
description: SaaS User
---
saas_user
---------

| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| apps        | Int          | &cross;      |
| createdAt   | String       | &check;      |
| devices     | Int          | &cross;      |
| email       | String       | &check;      |
| firstName   | String       | &check;      |
| id          | String       | &cross;      |
| isActive    | Boolean      | &cross;      |
| isDeleted   | Boolean      | &cross;      |
| isMonitored | Boolean      | &cross;      |
| issues      | Issues       | &cross;      |
| lastName    | String       | &check;      |
| phoneNumber | String       | &check;      |
| riskScore   | Double       | &cross;      |
| slackHandle | String       | &check;      |
| source      | Source       | &cross;      |
| teamIds     | List<String> | &cross;      |
| type        | String       | &cross;      |

#### Issues
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| critical | Int      | &cross;      |
| high     | Int      | &cross;      |
| low      | Int      | &cross;      |
| medium   | Int      | &cross;      |

#### Source
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| integrationId | String   | &cross;      |
| resourceId    | String   | &cross;      |
