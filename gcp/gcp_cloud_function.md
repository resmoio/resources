---
description: Google Cloud Platform Function
---
gcp_cloud_function
------------------

| **Name**                   | **Type**           | **Nullable** |
| -------------------------- | ------------------ | ------------ |
| buildEnvironmentVariables  | Map<String,String> | &check;      |
| buildId                    | String             | &check;      |
| buildName                  | String             | &check;      |
| buildWorkerPool            | String             | &check;      |
| description                | String             | &check;      |
| dockerRepository           | String             | &check;      |
| entryPoint                 | String             | &check;      |
| environmentVariables       | Map<String,String> | &check;      |
| eventTrigger               | EventTrigger       | &check;      |
| httpsTrigger               | HttpsTrigger       | &check;      |
| ingressSettings            | String             | &check;      |
| kmsKeyName                 | String             | &check;      |
| labels                     | Map<String,String> | &check;      |
| maxInstances               | Int                | &check;      |
| minInstances               | Int                | &check;      |
| name                       | String             | &cross;      |
| network                    | String             | &check;      |
| project                    | String             | &cross;      |
| runtime                    | String             | &check;      |
| secretEnvironmentVariables | List<SecretEnvVar> | &check;      |
| secretVolumes              | List<SecretVolume> | &check;      |
| serviceAccountEmail        | String             | &check;      |
| sourceArchiveUrl           | String             | &check;      |
| sourceRepository           | SourceRepository   | &check;      |
| sourceToken                | String             | &check;      |
| sourceUploadUrl            | String             | &cross;      |
| status                     | String             | &check;      |
| timeout                    | String             | &check;      |
| updateTime                 | String             | &check;      |
| versionId                  | Long               | &check;      |
| vpcConnector               | String             | &check;      |
| vpcConnectorEgressSettings | String             | &check;      |

#### EventTrigger
| **Name**      | **Type**                   | **Nullable** |
| ------------- | -------------------------- | ------------ |
| eventType     | String                     | &check;      |
| failurePolicy | EventTrigger.FailurePolicy | &check;      |
| resource      | String                     | &check;      |
| service       | String                     | &check;      |

#### EventTrigger.FailurePolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| action   | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### HttpsTrigger
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| securityLevel | String   | &check;      |
| url           | String   | &check;      |

#### SecretEnvVar
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| key       | String   | &check;      |
| projectId | String   | &check;      |
| secret    | String   | &check;      |
| version   | String   | &check;      |

#### SecretVolume
| **Name**  | **Type**                   | **Nullable** |
| --------- | -------------------------- | ------------ |
| mountPath | String                     | &check;      |
| projectId | String                     | &check;      |
| secret    | String                     | &check;      |
| versions  | SecretVolume.SecretVersion | &check;      |

#### SecretVolume.SecretVersion
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| path     | String   | &check;      |
| version  | String   | &check;      |

#### SourceRepository
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| deployedUrl | String   | &check;      |
| url         | String   | &check;      |
