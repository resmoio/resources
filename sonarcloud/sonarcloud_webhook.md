---
description: SonarCloud Webhook
---
sonarcloud_webhook
------------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| key            | String         | &cross;      |
| latestDelivery | LatestDelivery | &check;      |
| name           | String         | &check;      |
| projectKey     | String         | &check;      |
| secret         | String         | &check;      |
| url            | String         | &check;      |

#### LatestDelivery
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| at         | String   | &check;      |
| durationMs | Int      | &check;      |
| httpStatus | Int      | &check;      |
| id         | String   | &check;      |
| success    | Boolean  | &check;      |
