---
description: New Relic Muting Rule
---
newrelic_muting_rule
--------------------

| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| accountId     | Int      | &cross;      |
| createdAt     | String   | &cross;      |
| createdByUser | Int      | &check;      |
| description   | String   | &cross;      |
| enabled       | Boolean  | &cross;      |
| id            | String   | &cross;      |
| name          | String   | &cross;      |
| schedule      | Schedule | &check;      |
| status        | String   | &cross;      |
| updatedAt     | String   | &check;      |
| updatedByUser | Int      | &check;      |

#### Schedule
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| endRepeat        | String       | &check;      |
| endTime          | String       | &check;      |
| nextEndTime      | String       | &check;      |
| nextStartTime    | String       | &check;      |
| repeat           | String       | &check;      |
| repeatCount      | Int          | &check;      |
| startTime        | String       | &check;      |
| timeZone         | String       | &check;      |
| weeklyRepeatDays | List<String> | &check;      |
