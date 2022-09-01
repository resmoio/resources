---
description: Opsgenie Schedule
---
opsgenie_schedule
-----------------

| **Name**    | **Type**       | **Nullable** |
| ----------- | -------------- | ------------ |
| accountName | String         | &check;      |
| description | String         | &cross;      |
| enabled     | Boolean        | &cross;      |
| id          | String         | &cross;      |
| name        | String         | &cross;      |
| ownerTeam   | Team           | &cross;      |
| rotations   | List<Rotation> | &cross;      |
| timezone    | String         | &cross;      |

#### Rotation
| **Name**        | **Type**                   | **Nullable** |
| --------------- | -------------------------- | ------------ |
| id              | String                     | &cross;      |
| length          | Int                        | &cross;      |
| name            | String                     | &cross;      |
| participants    | List<Rotation.Participant> | &check;      |
| startDate       | String                     | &cross;      |
| timeRestriction | Rotation.TimeRestriction   | &check;      |
| type            | String                     | &cross;      |

#### Rotation.Participant
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| type     | String   | &check;      |
| username | String   | &check;      |

#### Rotation.TimeRestriction
| **Name**     | **Type**                                   | **Nullable** |
| ------------ | ------------------------------------------ | ------------ |
| restrictions | List<Rotation.TimeRestriction.Restriction> | &check;      |
| type         | String                                     | &check;      |

#### Rotation.TimeRestriction.Restriction
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| endHour   | Int      | &cross;      |
| endMin    | Int      | &cross;      |
| startHour | Int      | &cross;      |
| startMin  | Int      | &cross;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
