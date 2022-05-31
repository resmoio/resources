---
description: PagerDuty Schedule
---
pagerduty_schedule
------------------

| **Name**             | **Type**            | **Nullable** |
| -------------------- | ------------------- | ------------ |
| description          | String              | &check;      |
| escalationPolicies   | List<String>        | &check;      |
| finalSchedule        | FinalSchedule       | &check;      |
| id                   | String              | &cross;      |
| name                 | String              | &check;      |
| overridesSubSchedule | FinalSchedule       | &check;      |
| scheduleLayers       | List<ScheduleLayer> | &check;      |
| summary              | String              | &check;      |
| teams                | List<String>        | &check;      |
| timeZone             | String              | &check;      |
| type                 | String              | &check;      |
| users                | List<String>        | &check;      |

#### FinalSchedule
| **Name**                   | **Type**                    | **Nullable** |
| -------------------------- | --------------------------- | ------------ |
| name                       | String                      | &check;      |
| renderedCoveragePercentage | Number                      | &check;      |
| renderedScheduleEntries    | List<RenderedScheduleEntry> | &check;      |

#### RenderedScheduleEntry
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| end      | String   | &check;      |
| start    | String   | &check;      |
| user     | String   | &check;      |

#### ScheduleLayer
| **Name**                   | **Type**                        | **Nullable** |
| -------------------------- | ------------------------------- | ------------ |
| end                        | String                          | &check;      |
| id                         | String                          | &check;      |
| name                       | String                          | &check;      |
| renderedCoveragePercentage | Number                          | &check;      |
| renderedScheduleEntries    | List<RenderedScheduleEntry>     | &check;      |
| restrictions               | List<ScheduleLayer.Restriction> | &check;      |
| rotationTurnLengthSeconds  | Int                             | &check;      |
| rotationVirtualStart       | String                          | &check;      |
| start                      | String                          | &check;      |
| users                      | List<String>                    | &check;      |

#### ScheduleLayer.Restriction
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| durationSeconds | Int      | &check;      |
| startDayOfWeek  | Int      | &check;      |
| startTimeOfDay  | String   | &check;      |
| type            | String   | &check;      |
