---
description: Sentry Organization
---
sentry_organization
-------------------

| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| dateCreated      | String   | &check;      |
| id               | String   | &cross;      |
| isEarlyAdopter   | Boolean  | &check;      |
| organizationName | String   | &check;      |
| require2FA       | Boolean  | &check;      |
| slug             | String   | &cross;      |
| status           | Status   | &check;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
