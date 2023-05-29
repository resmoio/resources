---
description: Help Scout Team
---
helpscout_team
--------------

| **Name**  | **Type**                  | **Nullable** |
| --------- | ------------------------- | ------------ |
| createdAt | String                    | &check;      |
| id        | String                    | &cross;      |
| initials  | String                    | &check;      |
| members   | List<HelpScoutTeamMember> | &cross;      |
| mention   | String                    | &check;      |
| name      | String                    | &check;      |
| photoUrl  | String                    | &check;      |
| timezone  | String                    | &check;      |
| updatedAt | String                    | &check;      |

#### HelpScoutTeamMember
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| email     | String   | &check;      |
| firstName | String   | &check;      |
| id        | String   | &cross;      |
| jobTitle  | String   | &check;      |
| lastName  | String   | &check;      |
| role      | String   | &check;      |
| type      | String   | &check;      |
