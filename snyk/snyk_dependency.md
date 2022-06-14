---
description: Snyk Dependency
---
snyk_dependency
---------------

| **Name**                   | **Type**      | **Nullable** |
| -------------------------- | ------------- | ------------ |
| copyright                  | List<String>  | &check;      |
| dependenciesWithIssues     | List<String>  | &check;      |
| deprecatedVersions         | List<String>  | &check;      |
| firstPublishedDate         | String        | &check;      |
| id                         | String        | &cross;      |
| isDeprecated               | Boolean       | &check;      |
| latestVersion              | String        | &check;      |
| latestVersionPublishedDate | String        | &check;      |
| licenses                   | List<License> | &check;      |
| name                       | String        | &check;      |
| projects                   | List<Project> | &check;      |
| type                       | String        | &check;      |
| version                    | String        | &check;      |

#### License
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| license  | String   | &check;      |
| title    | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
