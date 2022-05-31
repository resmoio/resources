---
description: Opsgenie Notification Rule
---
opsgenie_notification_rule
--------------------------

| **Name**         | **Type**        | **Nullable** |
| ---------------- | --------------- | ------------ |
| accountName      | String          | &check;      |
| actionType       | String          | &check;      |
| id               | String          | &cross;      |
| name             | String          | &cross;      |
| notificationTime | List<String>    | &check;      |
| order            | Int             | &check;      |
| schedules        | List<Schedule>  | &check;      |
| steps            | List<Step>      | &check;      |
| timeRestriction  | TimeRestriction | &check;      |
| userId           | String          | &cross;      |

#### Schedule
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
| type     | String   | &cross;      |

#### Step
| **Name**  | **Type**       | **Nullable** |
| --------- | -------------- | ------------ |
| contact   | Step.Contact   | &cross;      |
| enabled   | Boolean        | &cross;      |
| sendAfter | Step.SendAfter | &check;      |

#### Step.Contact
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| method   | String   | &cross;      |
| to       | String   | &cross;      |

#### Step.SendAfter
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| timeAmount | Int      | &cross;      |
| timeUnit   | String   | &cross;      |

#### TimeRestriction
| **Name**    | **Type**                    | **Nullable** |
| ----------- | --------------------------- | ------------ |
| restriction | TimeRestriction.Restriction | &cross;      |
| type        | String                      | &cross;      |

#### TimeRestriction.Restriction
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| endHour   | Int      | &cross;      |
| endMin    | Int      | &cross;      |
| startHour | Int      | &cross;      |
| startMin  | Int      | &cross;      |
