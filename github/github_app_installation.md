---
description: GitHub App Installation
---
github_app_installation
-----------------------

| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| account                | Account      | &check;      |
| appId                  | Long         | &check;      |
| appSlug                | String       | &check;      |
| createdAt              | String       | &check;      |
| events                 | List<String> | &check;      |
| hasMultipleSingleFiles | Boolean      | &check;      |
| id                     | Long         | &cross;      |
| organization           | Organization | &check;      |
| permissions            | Permissions  | &check;      |
| repositorySelection    | String       | &check;      |
| singleFileName         | String       | &check;      |
| singleFilePaths        | List<String> | &check;      |
| suspendedAt            | String       | &check;      |
| suspendedBy            | String       | &check;      |
| targetId               | Long         | &check;      |
| targetType             | String       | &check;      |
| updatedAt              | String       | &check;      |

#### Account
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | Long     | &check;      |
| login     | String   | &check;      |
| nodeId    | String   | &check;      |
| siteAdmin | Boolean  | &check;      |
| type      | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### Permissions
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| actions                         | String   | &check;      |
| administration                  | String   | &check;      |
| checks                          | String   | &check;      |
| contents                        | String   | &check;      |
| deployments                     | String   | &check;      |
| discussions                     | String   | &check;      |
| environments                    | String   | &check;      |
| issues                          | String   | &check;      |
| members                         | String   | &check;      |
| metadata                        | String   | &check;      |
| organizationAdministration      | String   | &check;      |
| organizationAnnouncementBanners | String   | &check;      |
| organizationCustomRoles         | String   | &check;      |
| organizationHooks               | String   | &check;      |
| organizationPackages            | String   | &check;      |
| organizationPlan                | String   | &check;      |
| organizationProjects            | String   | &check;      |
| organizationSecrets             | String   | &check;      |
| organizationSelfHostedRunners   | String   | &check;      |
| organizationUserBlocking        | String   | &check;      |
| packages                        | String   | &check;      |
| pages                           | String   | &check;      |
| pullRequests                    | String   | &check;      |
| repositoryAnnouncementBanners   | String   | &check;      |
| repositoryHooks                 | String   | &check;      |
| repositoryProjects              | String   | &check;      |
| secretScanningAlerts            | String   | &check;      |
| secrets                         | String   | &check;      |
| securityEvents                  | String   | &check;      |
| singleFile                      | String   | &check;      |
| statuses                        | String   | &check;      |
| teamDiscussions                 | String   | &check;      |
| vulnerabilityAlerts             | String   | &check;      |
| workflows                       | String   | &check;      |
