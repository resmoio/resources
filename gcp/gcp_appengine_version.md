---
description: Google Cloud Platform AppEngine Version
---
gcp_appengine_version
---------------------

| **Name**                  | **Type**            | **Nullable** |
| ------------------------- | ------------------- | ------------ |
| apiConfig                 | ApiConfigHandler    | &check;      |
| automaticScaling          | AutomaticScaling    | &check;      |
| basicScaling              | BasicScaling        | &check;      |
| buildEnvVariables         | Map<String,String>  | &check;      |
| createTime                | String              | &check;      |
| createdBy                 | String              | &check;      |
| defaultExpiration         | String              | &check;      |
| endpointsApiService       | EndpointsApiService | &check;      |
| entrypoint                | Entrypoint          | &check;      |
| env                       | String              | &check;      |
| envVariables              | Map<String,String>  | &check;      |
| errorHandlers             | List<ErrorHandler>  | &check;      |
| handlers                  | List<UrlMap>        | &check;      |
| healthCheck               | HealthCheck         | &check;      |
| id                        | String              | &cross;      |
| inboundServices           | List<String>        | &check;      |
| instanceClass             | String              | &check;      |
| libraries                 | List<Library>       | &check;      |
| livenessCheck             | LivenessCheck       | &check;      |
| manualScaling             | ManualScaling       | &check;      |
| name                      | String              | &cross;      |
| network                   | Network             | &check;      |
| nobuildFilesRegex         | String              | &check;      |
| project                   | String              | &cross;      |
| readinessCheck            | ReadinessCheck      | &check;      |
| resources                 | Resources           | &check;      |
| runtime                   | String              | &check;      |
| runtimeApiVersion         | String              | &check;      |
| runtimeChannel            | String              | &check;      |
| runtimeMainExecutablePath | String              | &check;      |
| servingStatus             | String              | &check;      |
| threadsafe                | Boolean             | &check;      |
| versionUrl                | String              | &check;      |
| vm                        | Boolean             | &check;      |
| vpcAccessConnector        | VpcAccessConnector  | &check;      |
| zones                     | List<String>        | &check;      |

#### ApiConfigHandler
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| authFailAction | String   | &check;      |
| login          | String   | &check;      |
| script         | String   | &check;      |
| securityLevel  | String   | &check;      |
| url            | String   | &check;      |

#### AutomaticScaling
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| coolDownPeriod        | String   | &check;      |
| maxConcurrentRequests | Int      | &check;      |
| maxIdleInstances      | Int      | &check;      |
| maxPendingLatency     | String   | &check;      |
| maxTotalInstances     | Int      | &check;      |
| minIdleInstances      | Int      | &check;      |
| minPendingLatency     | String   | &check;      |
| minTotalInstances     | Int      | &check;      |

#### BasicScaling
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| idleTimeout  | String   | &check;      |
| maxInstances | Int      | &check;      |

#### EndpointsApiService
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| configId             | String   | &check;      |
| disableTraceSampling | Boolean  | &check;      |
| name                 | String   | &check;      |
| rolloutStrategy      | String   | &check;      |

#### Entrypoint
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| shell    | String   | &check;      |

#### ErrorHandler
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| errorCode  | String   | &check;      |
| mimeType   | String   | &check;      |
| staticFile | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### HealthCheck
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| checkInterval      | String   | &check;      |
| disableHealthCheck | Boolean  | &check;      |
| healthyThreshold   | Int      | &check;      |
| host               | String   | &check;      |
| restartThreshold   | Int      | &check;      |
| timeout            | String   | &check;      |
| unhealthyThreshold | Int      | &check;      |

#### Library
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| version  | String   | &check;      |

#### LivenessCheck
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| checkInterval    | String   | &check;      |
| failureThreshold | Int      | &check;      |
| host             | String   | &check;      |
| initialDelay     | String   | &check;      |
| path             | String   | &check;      |
| successThreshold | Int      | &check;      |
| timeout          | String   | &check;      |

#### ManualScaling
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| instances | Int      | &check;      |

#### Network
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| forwardedPorts  | List<String> | &check;      |
| instanceTag     | String       | &check;      |
| name            | String       | &check;      |
| sessionAffinity | Boolean      | &check;      |
| subnetworkName  | String       | &check;      |

#### ReadinessCheck
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| appStartTimeout  | String   | &check;      |
| checkInterval    | String   | &check;      |
| failureThreshold | Int      | &check;      |
| host             | String   | &check;      |
| path             | String   | &check;      |
| successThreshold | Int      | &check;      |
| timeout          | String   | &check;      |

#### Resources
| **Name** | **Type**               | **Nullable** |
| -------- | ---------------------- | ------------ |
| cpu      | Number                 | &check;      |
| diskGb   | Number                 | &check;      |
| memoryGb | Number                 | &check;      |
| volumes  | List<Resources.Volume> | &check;      |

#### Resources.Volume
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| name       | String   | &check;      |
| volumeType | String   | &check;      |

#### UrlMap
| **Name**                 | **Type**                  | **Nullable** |
| ------------------------ | ------------------------- | ------------ |
| apiEndpoint              | UrlMap.ApiEndpointHandler | &check;      |
| authFailAction           | String                    | &check;      |
| login                    | String                    | &check;      |
| redirectHttpResponseCode | String                    | &check;      |
| script                   | UrlMap.ScriptHandler      | &check;      |
| securityLevel            | String                    | &check;      |
| staticFiles              | UrlMap.StaticFilesHandler | &check;      |
| urlRegex                 | String                    | &check;      |

#### UrlMap.ApiEndpointHandler
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| scriptPath | String   | &check;      |

#### UrlMap.ScriptHandler
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| scriptPath | String   | &check;      |

#### UrlMap.StaticFilesHandler
| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| applicationReadable | Boolean            | &check;      |
| expiration          | String             | &check;      |
| httpHeaders         | Map<String,String> | &check;      |
| mimeType            | String             | &check;      |
| path                | String             | &check;      |
| requireMatchingFile | Boolean            | &check;      |
| uploadPathRegex     | String             | &check;      |

#### VpcAccessConnector
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| egressSetting | String   | &check;      |
| name          | String   | &check;      |
