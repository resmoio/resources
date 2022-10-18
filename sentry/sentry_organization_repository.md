---
description: Sentry Organization Repository
---
sentry_organization_repository
------------------------------

| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| dateCreated   | String       | &check;      |
| externalSlug  | String       | &check;      |
| id            | String       | &cross;      |
| integrationId | String       | &check;      |
| name          | String       | &cross;      |
| organization  | Organization | &cross;      |
| provider      | Provider     | &check;      |
| status        | String       | &check;      |
| url           | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &check;      |

#### Provider
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
