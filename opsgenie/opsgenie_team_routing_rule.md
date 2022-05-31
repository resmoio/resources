---
description: Opsgenie Team Routing Rule
---
opsgenie_team_routing_rule
--------------------------

| **Name**        | **Type**        | **Nullable** |
| --------------- | --------------- | ------------ |
| accountName     | String          | &check;      |
| criteria        | Criteria        | &check;      |
| id              | String          | &cross;      |
| isDefault       | Boolean         | &check;      |
| name            | String          | &cross;      |
| notify          | Notify          | &check;      |
| order           | Int             | &check;      |
| teamId          | String          | &cross;      |
| timeRestriction | TimeRestriction | &check;      |
| timezone        | String          | &check;      |

#### Criteria
| **Name**   | **Type**                 | **Nullable** |
| ---------- | ------------------------ | ------------ |
| conditions | List<Criteria.Condition> | &check;      |
| type       | String                   | &check;      |

#### Criteria.Condition
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| expectedValue | String   | &check;      |
| field         | String   | &check;      |
| key           | String   | &check;      |
| not           | Boolean  | &check;      |
| operation     | String   | &check;      |
| order         | Int      | &check;      |

#### Notify
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### TimeRestriction
| **Name**     | **Type**                          | **Nullable** |
| ------------ | --------------------------------- | ------------ |
| restriction  | TimeRestriction.Restriction       | &cross;      |
| restrictions | List<TimeRestriction.Restriction> | &check;      |
| type         | String                            | &check;      |

#### TimeRestriction.Restriction
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| endDay    | String   | &check;      |
| endHour   | Int      | &check;      |
| endMin    | Int      | &check;      |
| startDay  | String   | &check;      |
| startHour | Int      | &check;      |
| startMin  | Int      | &check;      |
