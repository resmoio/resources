---
description: GitLab Project
---
gitlab_project
--------------

| **Name**                                  | **Type**                  | **Nullable** |
| ----------------------------------------- | ------------------------- | ------------ |
| allowMergeOnSkippedPipeline               | String                    | &check;      |
| analyticsAccessLevel                      | String                    | &check;      |
| archived                                  | Boolean                   | &check;      |
| autoCancelPendingPipelines                | String                    | &check;      |
| autoDevopsDeployStrategy                  | String                    | &check;      |
| autoDevopsEnabled                         | Boolean                   | &check;      |
| autocloseReferencedIssues                 | Boolean                   | &check;      |
| buildCoverageRegex                        | String                    | &check;      |
| buildTimeout                              | Int                       | &check;      |
| buildsAccessLevel                         | String                    | &check;      |
| canCreateMergeRequestIn                   | Boolean                   | &check;      |
| ciConfigPath                              | String                    | &check;      |
| ciDefaultGitDepth                         | Int                       | &check;      |
| ciForwardDeploymentEnabled                | Boolean                   | &check;      |
| ciJobTokenScopeEnabled                    | Boolean                   | &check;      |
| complianceFrameworks                      | List<String>              | &cross;      |
| containerExpirationPolicy                 | ContainerExpirationPolicy | &check;      |
| containerRegistryAccessLevel              | String                    | &check;      |
| containerRegistryEnabled                  | Boolean                   | &check;      |
| containerRegistryImagePrefix              | String                    | &check;      |
| createdAt                                 | Date                      | &check;      |
| creatorId                                 | Int                       | &check;      |
| defaultBranch                             | String                    | &check;      |
| description                               | String                    | &check;      |
| emailsDisabled                            | String                    | &check;      |
| emptyRepo                                 | Boolean                   | &check;      |
| externalAuthorizationClassificationLabel  | String                    | &check;      |
| forkingAccessLevel                        | String                    | &check;      |
| forksCount                                | Int                       | &check;      |
| id                                        | String                    | &cross;      |
| importStatus                              | String                    | &check;      |
| issuesAccessLevel                         | String                    | &check;      |
| issuesEnabled                             | Boolean                   | &check;      |
| jobsEnabled                               | Boolean                   | &check;      |
| keepLatestArtifact                        | Boolean                   | &check;      |
| lastActivityAt                            | Date                      | &check;      |
| lfsEnabled                                | Boolean                   | &check;      |
| mergeCommitTemplate                       | String                    | &check;      |
| mergeMethod                               | String                    | &check;      |
| mergeRequestsAccessLevel                  | String                    | &check;      |
| mergeRequestsEnabled                      | Boolean                   | &check;      |
| name                                      | String                    | &check;      |
| nameWithNamespace                         | String                    | &check;      |
| namespace                                 | Namespace                 | &check;      |
| onlyAllowMergeIfAllDiscussionsAreResolved | Boolean                   | &check;      |
| onlyAllowMergeIfPipelineSucceeds          | Boolean                   | &check;      |
| openIssuesCount                           | Int                       | &check;      |
| operationsAccessLevel                     | String                    | &check;      |
| packagesEnabled                           | Boolean                   | &check;      |
| pagesAccessLevel                          | String                    | &check;      |
| path                                      | String                    | &check;      |
| pathWithNamespace                         | String                    | &check;      |
| permissions                               | Permissions               | &check;      |
| printingMergeRequestLinkEnabled           | Boolean                   | &check;      |
| publicJobs                                | Boolean                   | &check;      |
| removeSourceBranchAfterMerge              | Boolean                   | &check;      |
| repositoryAccessLevel                     | String                    | &check;      |
| requestAccessEnabled                      | Boolean                   | &check;      |
| requirementsEnabled                       | Boolean                   | &check;      |
| resolveOutdatedDiffDiscussions            | Boolean                   | &check;      |
| restrictUserDefinedVariables              | Boolean                   | &check;      |
| securityAndComplianceEnabled              | Boolean                   | &check;      |
| serviceDeskAddress                        | String                    | &check;      |
| serviceDeskEnabled                        | Boolean                   | &check;      |
| sharedRunnersEnabled                      | Boolean                   | &check;      |
| sharedWithGroups                          | List<String>              | &cross;      |
| snippetsAccessLevel                       | String                    | &check;      |
| snippetsEnabled                           | Boolean                   | &check;      |
| squashCommitTemplate                      | String                    | &check;      |
| squashOption                              | String                    | &check;      |
| starCount                                 | Int                       | &check;      |
| suggestionCommitMessage                   | String                    | &check;      |
| tagList                                   | List<String>              | &cross;      |
| topics                                    | List<String>              | &cross;      |
| visibility                                | String                    | &check;      |
| webUrl                                    | String                    | &check;      |
| wikiAccessLevel                           | String                    | &check;      |
| wikiEnabled                               | Boolean                   | &check;      |

#### ContainerExpirationPolicy
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| cadence       | String   | &check;      |
| enabled       | Boolean  | &check;      |
| keepN         | Int      | &check;      |
| nameRegex     | String   | &check;      |
| nameRegexKeep | String   | &check;      |
| nextRunAt     | Date     | &check;      |
| olderThan     | String   | &check;      |

#### Namespace
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| fullPath | String   | &check;      |
| id       | Int      | &check;      |
| kind     | String   | &check;      |
| name     | String   | &check;      |
| parentId | String   | &check;      |
| path     | String   | &check;      |

#### Permissions
| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| groupAccess   | Permissions.Access | &check;      |
| projectAccess | Permissions.Access | &check;      |

#### Permissions.Access
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| accessLevel       | Int      | &check;      |
| notificationLevel | String   | &check;      |
