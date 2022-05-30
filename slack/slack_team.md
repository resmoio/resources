---
description: Slack Team
---
slack_team
----------

| **Name**         | **Type**        | **Nullable** |
| ---------------- | --------------- | ------------ |
| billingPlan      | String          | &check;      |
| defaultChannels  | List<String>    | &check;      |
| discoverable     | String          | &check;      |
| domain           | String          | &check;      |
| emailDomain      | String          | &check;      |
| enterpriseDomain | String          | &check;      |
| enterpriseId     | String          | &check;      |
| enterpriseName   | String          | &check;      |
| fields           | List<TeamField> | &check;      |
| id               | String          | &cross;      |
| isVerified       | Boolean         | &check;      |
| name             | String          | &cross;      |
| preferences      | TeamPreferences | &check;      |
| url              | String          | &check;      |

#### TeamField
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| fieldName      | String       | &check;      |
| hint           | String       | &check;      |
| id             | String       | &check;      |
| isHidden       | Boolean      | &check;      |
| isProtected    | Boolean      | &check;      |
| label          | String       | &check;      |
| ordering       | Int          | &check;      |
| possibleValues | List<String> | &check;      |
| type           | String       | &check;      |

#### TeamPreferences
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| allowMessageDeletion | Boolean  | &check;      |
| disableFileUploads   | String   | &check;      |
| displayRealNames     | Boolean  | &check;      |
| msgEditWindowMins    | Int      | &check;      |
| whoCanPostGeneral    | String   | &check;      |
