---
description: SonarCloud Project
---
sonarcloud_project
------------------

| **Name**         | **Type**   | **Nullable** |
| ---------------- | ---------- | ------------ |
| key              | String     | &cross;      |
| lastAnalysisDate | String     | &check;      |
| links            | List<Link> | &check;      |
| name             | String     | &check;      |
| organization     | String     | &cross;      |
| qualifier        | String     | &check;      |
| revision         | String     | &check;      |
| visibility       | String     | &check;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| url      | String   | &check;      |
