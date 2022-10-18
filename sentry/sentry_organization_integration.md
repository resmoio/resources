---
description: Sentry Organization Integration
---
sentry_organization_integration
-------------------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| app          | App          | &check;      |
| organization | Organization | &check;      |
| status       | String       | &check;      |
| uuid         | String       | &cross;      |

#### App
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &cross;      |
| uuid     | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| slug     | String   | &cross;      |
