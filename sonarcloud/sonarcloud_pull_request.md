---
description: SonarCloud Pull Request
---
sonarcloud_pull_request
-----------------------

| **Name**     | **Type**          | **Nullable** |
| ------------ | ----------------- | ------------ |
| analysisDate | String            | &check;      |
| base         | String            | &check;      |
| branch       | String            | &check;      |
| commit       | Commit            | &check;      |
| contributors | List<Contributor> | &check;      |
| key          | String            | &cross;      |
| projectKey   | String            | &check;      |
| status       | Status            | &check;      |
| target       | String            | &check;      |
| title        | String            | &check;      |
| url          | String            | &check;      |

#### Commit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| sha      | String   | &check;      |

#### Contributor
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| login    | String   | &cross;      |
| name     | String   | &check;      |

#### Status
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| bugs              | Int      | &check;      |
| codeSmells        | Int      | &check;      |
| qualityGateStatus | String   | &check;      |
| vulnerabilities   | Int      | &check;      |
