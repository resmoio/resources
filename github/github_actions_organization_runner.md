---
description: GitHub Actions Organization Self-Hosted Runner
---
github_actions_organization_runner
----------------------------------

| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| busy          | Boolean      | &check;      |
| id            | String       | &cross;      |
| labels        | List<Label>  | &check;      |
| name          | String       | &check;      |
| organization  | Organization | &cross;      |
| os            | String       | &check;      |
| runnerGroupId | String       | &check;      |
| status        | String       | &check;      |

#### Label
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
