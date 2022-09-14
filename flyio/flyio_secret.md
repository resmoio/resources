---
description: Flyio Secret
---
flyio_secret
------------

| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| appId          | String   | &cross;      |
| appName        | String   | &cross;      |
| createdAt      | String   | &cross;      |
| digest         | String   | &cross;      |
| id             | String   | &cross;      |
| name           | String   | &cross;      |
| organizationId | String   | &cross;      |
| user           | User     | &cross;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| id       | String   | &check;      |
| name     | String   | &check;      |
| username | String   | &check;      |
