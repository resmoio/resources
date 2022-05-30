---
description: PagerDuty User
---
pagerduty_user
--------------

| **Name**          | **Type**                   | **Nullable** |
| ----------------- | -------------------------- | ------------ |
| color             | String                     | &check;      |
| contactMethods    | List<UserContactMethod>    | &check;      |
| description       | String                     | &check;      |
| email             | String                     | &check;      |
| id                | String                     | &cross;      |
| invitationSent    | Boolean                    | &check;      |
| jobTitle          | String                     | &check;      |
| name              | String                     | &check;      |
| notificationRules | List<UserNotificationRule> | &check;      |
| role              | String                     | &check;      |
| subdomains        | List<String>               | &check;      |
| summary           | String                     | &check;      |
| teams             | List<String>               | &check;      |
| timeZone          | String                     | &check;      |
| type              | String                     | &check;      |

#### UserContactMethod
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| address     | String   | &check;      |
| blacklisted | Boolean  | &check;      |
| countryCode | Int      | &check;      |
| enabled     | Boolean  | &check;      |
| id          | String   | &check;      |
| label       | String   | &check;      |
| summary     | String   | &check;      |
| type        | String   | &check;      |

#### UserNotificationRule
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| contactMethod       | String   | &check;      |
| id                  | String   | &check;      |
| startDelayInMinutes | Int      | &check;      |
| summary             | String   | &check;      |
| type                | String   | &check;      |
| urgency             | String   | &check;      |
