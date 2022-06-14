---
description: Snyk Issue
---
snyk_issue
----------

| **Name**             | **Type**      | **Nullable** |
| -------------------- | ------------- | ------------ |
| CVSSv3               | String        | &check;      |
| credit               | List<String>  | &check;      |
| cvssScore            | String        | &check;      |
| disclosureTime       | String        | &check;      |
| exploitMaturity      | String        | &check;      |
| fixedDate            | String        | &check;      |
| id                   | String        | &cross;      |
| identifiers          | Identifiers   | &check;      |
| ignored              | List<Ignored> | &check;      |
| introducedDate       | String        | &check;      |
| isFixed              | Boolean       | &check;      |
| isPatchable          | Boolean       | &check;      |
| isPatched            | Boolean       | &check;      |
| isPinnable           | Boolean       | &check;      |
| isUpgradable         | Boolean       | &check;      |
| jiraIssueUrl         | String        | &check;      |
| language             | String        | &check;      |
| originalSeverity     | String        | &check;      |
| package              | String        | &check;      |
| packageManager       | String        | &check;      |
| patchedDate          | String        | &check;      |
| patches              | List<Patch>   | &check;      |
| priorityScore        | Int           | &check;      |
| projects             | List<Project> | &check;      |
| publicationTime      | String        | &check;      |
| semver               | Semver        | &check;      |
| severity             | String        | &check;      |
| title                | String        | &check;      |
| type                 | String        | &check;      |
| uniqueSeveritiesList | List<String>  | &check;      |
| url                  | String        | &check;      |
| version              | String        | &check;      |

#### Identifiers
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| cve      | List<String> | &check;      |
| cwe      | List<String> | &check;      |
| osvdb    | List<String> | &check;      |

#### Ignored
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| expires  | String   | &check;      |
| reason   | String   | &check;      |
| source   | String   | &check;      |

#### Patch
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| comments         | List<String> | &check;      |
| id               | String       | &check;      |
| modificationTime | String       | &check;      |
| urls             | List<String> | &check;      |
| version          | String       | &check;      |

#### Project
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| id             | String   | &check;      |
| name           | String   | &check;      |
| packageManager | String   | &check;      |
| source         | String   | &check;      |
| targetFile     | String   | &check;      |
| url            | String   | &check;      |

#### Semver
| **Name**   | **Type**     | **Nullable** |
| ---------- | ------------ | ------------ |
| unaffected | String       | &check;      |
| vulnerable | List<String> | &check;      |
