---
description: Sentry Team Project
---
sentry_team_project
-------------------

| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| dateCreated   | String       | &check;      |
| features      | List<String> | &check;      |
| firstEvent    | String       | &check;      |
| hasAccess     | Boolean      | &check;      |
| id            | String       | &cross;      |
| isBookmarked  | Boolean      | &check;      |
| isMember      | Boolean      | &check;      |
| latestDeploys | String       | &check;      |
| name          | String       | &check;      |
| organization  | Organization | &check;      |
| platform      | String       | &check;      |
| slug          | String       | &check;      |
| team          | Team         | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &check;      |

#### Team
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &check;      |
