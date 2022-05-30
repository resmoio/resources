---
description: PagerDuty Service
---
pagerduty_service
-----------------

| **Name**                         | **Type**                         | **Nullable** |
| -------------------------------- | -------------------------------- | ------------ |
| acknowledgementTimeout           | Int                              | &check;      |
| addons                           | List<String>                     | &check;      |
| alertCreation                    | String                           | &check;      |
| alertGroupingParameters          | AlertGroupingParameters          | &check;      |
| autoPauseNotificationsParameters | AutoPauseNotificationsParameters | &check;      |
| autoResolveTimeout               | Int                              | &check;      |
| createdAt                        | String                           | &check;      |
| description                      | String                           | &check;      |
| escalationPolicy                 | String                           | &check;      |
| id                               | String                           | &cross;      |
| incidentUrgencyRule              | IncidentUrgencyRule              | &check;      |
| integrations                     | List<Integration>                | &check;      |
| name                             | String                           | &check;      |
| responsePlay                     | String                           | &check;      |
| scheduledActions                 | List<ScheduledAction>            | &check;      |
| status                           | String                           | &check;      |
| summary                          | String                           | &check;      |
| supportHours                     | SupportHours                     | &check;      |
| teams                            | List<String>                     | &check;      |
| type                             | String                           | &check;      |

#### AlertGroupingParameters
| **Name** | **Type**                       | **Nullable** |
| -------- | ------------------------------ | ------------ |
| config   | AlertGroupingParameters.Config | &check;      |
| type     | String                         | &check;      |

#### AlertGroupingParameters.Config
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| aggregate | String   | &check;      |
| fields    | String   | &check;      |
| timeout   | String   | &check;      |

#### AutoPauseNotificationsParameters
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |
| timeout  | Int      | &check;      |

#### IncidentUrgencyRule
| **Name**            | **Type**                         | **Nullable** |
| ------------------- | -------------------------------- | ------------ |
| duringSupportHours  | IncidentUrgencyRule.SupportHours | &check;      |
| outsideSupportHours | IncidentUrgencyRule.SupportHours | &check;      |
| type                | String                           | &check;      |
| urgency             | String                           | &check;      |

#### IncidentUrgencyRule.SupportHours
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| urgency  | String   | &check;      |

#### Integration
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| summary  | String   | &check;      |
| type     | String   | &check;      |

#### ScheduledAction
| **Name**  | **Type**           | **Nullable** |
| --------- | ------------------ | ------------ |
| at        | ScheduledAction.At | &check;      |
| toUrgency | String             | &check;      |
| type      | String             | &check;      |

#### ScheduledAction.At
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### SupportHours
| **Name**   | **Type**  | **Nullable** |
| ---------- | --------- | ------------ |
| daysOfWeek | List<Int> | &check;      |
| endTime    | String    | &check;      |
| startTime  | String    | &check;      |
| timeZone   | String    | &check;      |
| type       | String    | &check;      |
