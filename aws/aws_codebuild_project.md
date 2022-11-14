---
description: Amazon Web Services CodeBuild Project
---
aws_codebuild_project
---------------------

| **Name**                | **Type**                        | **Nullable** |
| ----------------------- | ------------------------------- | ------------ |
| accountId               | String                          | &cross;      |
| accountName             | String                          | &check;      |
| arn                     | String                          | &cross;      |
| artifacts               | ProjectArtifacts                | &check;      |
| badge                   | ProjectBadge                    | &check;      |
| buildBatchConfig        | ProjectBuildBatchConfig         | &check;      |
| cache                   | ProjectCache                    | &check;      |
| concurrentBuildLimit    | Int                             | &check;      |
| created                 | String                          | &check;      |
| description             | String                          | &check;      |
| encryptionKey           | String                          | &check;      |
| environment             | ProjectEnvironment              | &check;      |
| fileSystemLocations     | List<ProjectFileSystemLocation> | &check;      |
| lastModified            | String                          | &check;      |
| logsConfig              | LogsConfig                      | &check;      |
| name                    | String                          | &check;      |
| projectVisibility       | String                          | &check;      |
| publicProjectAlias      | String                          | &check;      |
| queuedTimeoutInMinutes  | Int                             | &check;      |
| region                  | String                          | &cross;      |
| resourceAccessRole      | String                          | &check;      |
| secondaryArtifacts      | List<ProjectArtifacts>          | &check;      |
| secondarySourceVersions | List<ProjectSourceVersion>      | &check;      |
| secondarySources        | List<ProjectSource>             | &check;      |
| serviceRole             | String                          | &check;      |
| source                  | ProjectSource                   | &check;      |
| sourceVersion           | String                          | &check;      |
| tags                    | Map<String,String>              | &check;      |
| timeoutInMinutes        | Int                             | &check;      |
| vpcConfig               | VpcConfig                       | &check;      |
| webhook                 | Webhook                         | &check;      |

#### BatchRestrictions
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| computeTypesAllowed  | List<String> | &cross;      |
| maximumBuildsAllowed | Int          | &cross;      |

#### BuildStatusConfig
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| context   | String   | &check;      |
| targetUrl | String   | &check;      |

#### CloudWatchLogsConfig
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| groupName  | String   | &check;      |
| status     | String   | &check;      |
| streamName | String   | &check;      |

#### EnvironmentVariable
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |
| value    | String   | &check;      |

#### GitSubmodulesConfig
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| fetchSubmodules | Boolean  | &check;      |

#### LogsConfig
| **Name**       | **Type**             | **Nullable** |
| -------------- | -------------------- | ------------ |
| cloudWatchLogs | CloudWatchLogsConfig | &check;      |
| s3Logs         | S3LogsConfig         | &check;      |

#### ProjectArtifacts
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| artifactIdentifier   | String   | &check;      |
| bucketOwnerAccess    | String   | &check;      |
| encryptionDisabled   | Boolean  | &check;      |
| location             | String   | &check;      |
| name                 | String   | &check;      |
| namespaceType        | String   | &check;      |
| overrideArtifactName | Boolean  | &check;      |
| packaging            | String   | &check;      |
| path                 | String   | &check;      |
| type                 | String   | &check;      |

#### ProjectBadge
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| badgeEnabled    | Boolean  | &check;      |
| badgeRequestUrl | String   | &check;      |

#### ProjectBuildBatchConfig
| **Name**         | **Type**          | **Nullable** |
| ---------------- | ----------------- | ------------ |
| batchReportMode  | String            | &check;      |
| combineArtifacts | Boolean           | &check;      |
| restrictions     | BatchRestrictions | &check;      |
| serviceRole      | String            | &check;      |
| timeoutInMins    | Int               | &check;      |

#### ProjectCache
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| location | String       | &check;      |
| modes    | List<String> | &check;      |
| type     | String       | &check;      |

#### ProjectEnvironment
| **Name**                 | **Type**                  | **Nullable** |
| ------------------------ | ------------------------- | ------------ |
| certificate              | String                    | &check;      |
| computeType              | String                    | &check;      |
| environmentVariables     | List<EnvironmentVariable> | &check;      |
| image                    | String                    | &check;      |
| imagePullCredentialsType | String                    | &check;      |
| privilegedMode           | Boolean                   | &check;      |
| type                     | String                    | &check;      |

#### ProjectFileSystemLocation
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| identifier   | String   | &check;      |
| location     | String   | &check;      |
| mountOptions | String   | &check;      |
| mountPoint   | String   | &check;      |
| type         | String   | &check;      |

#### ProjectSource
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| auth                | SourceAuth          | &check;      |
| buildStatusConfig   | BuildStatusConfig   | &check;      |
| buildspec           | String              | &check;      |
| gitCloneDepth       | Int                 | &check;      |
| gitSubmodulesConfig | GitSubmodulesConfig | &check;      |
| insecureSsl         | Boolean             | &check;      |
| location            | String              | &check;      |
| reportBuildStatus   | Boolean             | &check;      |
| sourceIdentifier    | String              | &check;      |
| type                | String              | &check;      |

#### ProjectSourceVersion
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| sourceIdentifier | String   | &check;      |
| sourceVersion    | String   | &check;      |

#### S3LogsConfig
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| bucketOwnerAccess  | String   | &check;      |
| encryptionDisabled | Boolean  | &check;      |
| location           | String   | &check;      |
| status             | String   | &check;      |

#### SourceAuth
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| resource | String   | &check;      |
| type     | String   | &check;      |

#### VpcConfig
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| securityGroupIds | List<String> | &check;      |
| subnets          | List<String> | &check;      |
| vpcId            | String       | &check;      |

#### Webhook
| **Name**           | **Type**   | **Nullable** |
| ------------------ | ---------- | ------------ |
| branchFilter       | String     | &check;      |
| buildType          | String     | &check;      |
| filterGroups       | List<List> | &check;      |
| lastModifiedSecret | String     | &check;      |
| payloadUrl         | String     | &check;      |
| secret             | String     | &check;      |
| url                | String     | &check;      |

#### WebhookFilter
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| excludeMatchedPattern | Boolean  | &check;      |
| pattern               | String   | &check;      |
| type                  | String   | &check;      |
