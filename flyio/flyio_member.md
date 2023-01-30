---
description: Flyio Member
---
flyio_member
------------

| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| createdAt           | String       | &check;      |
| email               | String       | &check;      |
| featureFlags        | List<String> | &cross;      |
| id                  | String       | &cross;      |
| lastRegion          | String       | &check;      |
| organization        | Organization | &cross;      |
| trust               | String       | &check;      |
| twoFactorProtection | Boolean      | &check;      |
| username            | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
| slug     | String   | &cross;      |
