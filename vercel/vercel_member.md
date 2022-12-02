---
description: Vercel Member
---
vercel_member
-------------

| **Name**          | **Type**   | **Nullable** |
| ----------------- | ---------- | ------------ |
| accessRequestedAt | Long       | &check;      |
| bitbucket         | VCSInfo    | &check;      |
| confirmed         | Boolean    | &check;      |
| createdAt         | Long       | &check;      |
| email             | String     | &check;      |
| github            | VCSInfo    | &check;      |
| gitlab            | VCSInfo    | &check;      |
| joinedFrom        | JoinedFrom | &check;      |
| role              | String     | &check;      |
| uid               | String     | &cross;      |
| username          | String     | &check;      |

#### JoinedFrom
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| origin   | String   | &check;      |

#### VCSInfo
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| accountId | String   | &check;      |
| email     | String   | &check;      |
| login     | String   | &check;      |
| userId    | String   | &check;      |
