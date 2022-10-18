---
description: Sentry Organization Team
---
sentry_organization_team
------------------------

| **Name**     | **Type**      | **Nullable** |
| ------------ | ------------- | ------------ |
| dateCreated  | String        | &check;      |
| hasAccess    | Boolean       | &check;      |
| id           | String        | &cross;      |
| isMember     | Boolean       | &check;      |
| isPending    | Boolean       | &check;      |
| memberCount  | Int           | &check;      |
| organization | Organization  | &check;      |
| projects     | List<Project> | &check;      |
| slug         | String        | &cross;      |
| teamName     | String        | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &cross;      |

#### Project
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| dateCreated  | String       | &check;      |
| features     | List<String> | &check;      |
| firstEvent   | String       | &check;      |
| hasAccess    | Boolean      | &check;      |
| id           | String       | &cross;      |
| isBookmarked | Boolean      | &check;      |
| isInternal   | Boolean      | &check;      |
| isMember     | Boolean      | &check;      |
| isPublic     | Boolean      | &check;      |
| name         | String       | &check;      |
| platform     | String       | &check;      |
| slug         | String       | &cross;      |
| status       | String       | &check;      |
