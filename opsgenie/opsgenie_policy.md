---
description: Opsgenie Policy
---
opsgenie_policy
---------------

| **Name**                 | **Type**            | **Nullable** |
| ------------------------ | ------------------- | ------------ |
| accountName              | String              | &check;      |
| alias                    | String              | &check;      |
| autoCloseAction          | AutoCloseAction     | &check;      |
| autoRestartAction        | AutoRestartAction   | &check;      |
| continue                 | Boolean             | &check;      |
| deduplicationAction      | DeduplicationAction | &check;      |
| delayAction              | DelayAction         | &check;      |
| description              | String              | &check;      |
| enabled                  | Boolean             | &cross;      |
| filter                   | Filter              | &check;      |
| id                       | String              | &cross;      |
| ignoreOriginalResponders | Boolean             | &check;      |
| ignoreOriginalTags       | Boolean             | &check;      |
| message                  | String              | &check;      |
| name                     | String              | &cross;      |
| order                    | Int                 | &cross;      |
| policyDescription        | String              | &check;      |
| responders               | List<Responder>     | &check;      |
| scope                    | String              | &cross;      |
| suppress                 | Boolean             | &check;      |
| tags                     | List<String>        | &check;      |
| teamId                   | String              | &check;      |
| timeRestrictions         | TimeRestrictions    | &check;      |
| type                     | String              | &cross;      |

#### AutoCloseAction
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| duration | Duration | &cross;      |

#### AutoRestartAction
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| duration       | Duration | &check;      |
| maxRepeatCount | Int      | &check;      |

#### DeduplicationAction
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| count                   | Int      | &check;      |
| deduplicationActionType | String   | &check;      |
| duration                | Duration | &check;      |

#### DelayAction
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| delayOption | String   | &check;      |
| duration    | Duration | &check;      |
| untilHour   | Int      | &check;      |
| untilMinute | Int      | &check;      |

#### Duration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| timeAmount | Int      | &check;      |
| timeUnit   | String   | &check;      |

#### Filter
| **Name**   | **Type**               | **Nullable** |
| ---------- | ---------------------- | ------------ |
| conditions | List<Filter.Condition> | &check;      |
| type       | String                 | &check;      |

#### Filter.Condition
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| expectedValue | String   | &check;      |
| field         | String   | &check;      |
| key           | String   | &check;      |
| not           | Boolean  | &check;      |
| operation     | String   | &check;      |
| order         | Int      | &check;      |

#### Responder
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| type     | String   | &cross;      |

#### TimeRestrictions
| **Name**     | **Type**                           | **Nullable** |
| ------------ | ---------------------------------- | ------------ |
| restriction  | TimeRestrictions.Restriction       | &check;      |
| restrictions | List<TimeRestrictions.Restriction> | &check;      |
| type         | String                             | &check;      |

#### TimeRestrictions.Restriction
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| endDay    | String   | &check;      |
| endHour   | Int      | &check;      |
| endMin    | Int      | &check;      |
| startDay  | String   | &check;      |
| startHour | Int      | &check;      |
| startMin  | Int      | &check;      |
