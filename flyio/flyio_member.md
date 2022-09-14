---
description: Flyio Member
---
flyio_member
------------

| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| createdAt           | String       | &cross;      |
| email               | String       | &cross;      |
| featureFlags        | List<String> | &cross;      |
| id                  | String       | &cross;      |
| lastRegion          | String       | &check;      |
| organization        | Organization | &cross;      |
| trust               | String       | &check;      |
| twoFactorProtection | Boolean      | &cross;      |
| username            | String       | &cross;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
| slug     | String   | &cross;      |
