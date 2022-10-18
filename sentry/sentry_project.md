---
description: Sentry Project
---
sentry_project
--------------

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
| organization | Organization | &check;      |
| platform     | String       | &check;      |
| slug         | String       | &check;      |
| status       | String       | &check;      |

#### Organization
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| dateCreated    | String   | &check;      |
| id             | String   | &cross;      |
| isEarlyAdopter | Boolean  | &check;      |
| name           | String   | &check;      |
| require2FA     | Boolean  | &check;      |
| slug           | String   | &cross;      |
| status         | Status   | &check;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| status   | String   | &check;      |
