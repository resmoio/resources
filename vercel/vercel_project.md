---
description: Vercel Project
---
vercel_project
--------------

| **Name**                        | **Type**             | **Nullable** |
| ------------------------------- | -------------------- | ------------ |
| accountId                       | String               | &check;      |
| autoExposeSystemEnvs            | Boolean              | &check;      |
| buildCommand                    | String               | &check;      |
| commandForIgnoringBuildStep     | String               | &check;      |
| createdAt                       | Long                 | &check;      |
| devCommand                      | String               | &check;      |
| directoryListing                | Boolean              | &check;      |
| enablePreviewFeedback           | Boolean              | &check;      |
| framework                       | String               | &check;      |
| gitForkProtection               | Boolean              | &check;      |
| hasFloatingAliases              | Boolean              | &check;      |
| id                              | String               | &cross;      |
| installCommand                  | String               | &check;      |
| latestDeployments               | List<DeploymentInfo> | &check;      |
| link                            | Link                 | &check;      |
| live                            | Boolean              | &check;      |
| name                            | String               | &check;      |
| nodeVersion                     | String               | &check;      |
| outputDirectory                 | String               | &check;      |
| passwordProtection              | String               | &check;      |
| publicSource                    | Boolean              | &check;      |
| rootDirectory                   | String               | &check;      |
| serverlessFunctionRegion        | String               | &check;      |
| skipGitConnectDuringLink        | Boolean              | &check;      |
| sourceFilesOutsideRootDirectory | Boolean              | &check;      |
| ssoProtection                   | Map<String,String>   | &check;      |
| transferCompletedAt             | Long                 | &check;      |
| transferStartedAt               | Long                 | &check;      |
| transferToAccountId             | String               | &check;      |
| transferredFromAccountId        | String               | &check;      |
| updatedAt                       | Long                 | &check;      |

#### DeploymentInfo
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| alias              | List<String>       | &check;      |
| aliasAssigned      | Long               | &check;      |
| aliasError         | Map<String,String> | &check;      |
| aliasFinal         | String             | &check;      |
| automaticAliases   | List<String>       | &check;      |
| buildingAt         | Long               | &check;      |
| builds             | List<Map>          | &check;      |
| checksConclusion   | String             | &check;      |
| checksState        | String             | &check;      |
| createdAt          | Long               | &check;      |
| createdIn          | String             | &check;      |
| creator            | Map<String,String> | &check;      |
| deploymentHostname | String             | &check;      |
| forced             | Boolean            | &check;      |
| id                 | String             | &check;      |
| meta               | Map<String,String> | &check;      |
| monorepoManager    | String             | &check;      |
| name               | String             | &check;      |
| plan               | String             | &check;      |
| private            | Boolean            | &check;      |
| readyAt            | Long               | &check;      |
| readyState         | String             | &check;      |
| requestedAt        | Long               | &check;      |
| target             | String             | &check;      |
| teamId             | String             | &check;      |
| type               | String             | &check;      |
| url                | String             | &check;      |
| userId             | String             | &check;      |
| withCache          | Boolean            | &check;      |

#### Link
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| createdAt                | Long     | &check;      |
| gitCredentialId          | String   | &check;      |
| name                     | String   | &check;      |
| org                      | String   | &check;      |
| owner                    | String   | &check;      |
| productionBranch         | String   | &check;      |
| projectId                | String   | &check;      |
| projectName              | String   | &check;      |
| projectNameWithNamespace | String   | &check;      |
| projectNamespace         | String   | &check;      |
| projectUrl               | String   | &check;      |
| repo                     | String   | &check;      |
| repoId                   | Long     | &check;      |
| slug                     | String   | &check;      |
| sourceless               | Boolean  | &check;      |
| type                     | String   | &check;      |
| updatedAt                | Long     | &check;      |
| uuid                     | String   | &check;      |
| workspaceUuid            | String   | &check;      |
