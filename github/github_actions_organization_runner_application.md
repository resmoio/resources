---
description: GitHub Actions Organization Runner Application
---
github_actions_organization_runner_application
----------------------------------------------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| architecture      | String       | &check;      |
| downloadUrl       | String       | &check;      |
| filename          | String       | &cross;      |
| organization      | Organization | &cross;      |
| os                | String       | &cross;      |
| sha256Checksum    | String       | &check;      |
| tempDownloadToken | String       | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
