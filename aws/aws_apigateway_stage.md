---
description: Amazon Web Services ApiGateway Stage
---
aws_apigateway_stage
--------------------

| **Name**             | **Type**                  | **Nullable** |
| -------------------- | ------------------------- | ------------ |
| accessLogSettings    | AccessLogSettings         | &check;      |
| accountId            | String                    | &cross;      |
| apiId                | String                    | &check;      |
| cacheClusterEnabled  | Boolean                   | &check;      |
| cacheClusterSize     | String                    | &check;      |
| cacheClusterStatus   | String                    | &check;      |
| canarySettings       | CanarySettings            | &check;      |
| clientCertificateId  | String                    | &check;      |
| createdDate          | String                    | &check;      |
| deploymentId         | String                    | &check;      |
| description          | String                    | &check;      |
| documentationVersion | String                    | &check;      |
| lastUpdatedDate      | String                    | &check;      |
| methodSettings       | Map<String,MethodSetting> | &check;      |
| region               | String                    | &cross;      |
| stageName            | String                    | &cross;      |
| tags                 | Map<String,String>        | &check;      |
| tracingEnabled       | Boolean                   | &check;      |
| variables            | Map<String,String>        | &check;      |
| webAclArn            | String                    | &check;      |

#### AccessLogSettings
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| destinationArn | String   | &check;      |
| format         | String   | &check;      |

#### CanarySettings
| **Name**               | **Type**           | **Nullable** |
| ---------------------- | ------------------ | ------------ |
| deploymentId           | String             | &check;      |
| percentTraffic         | Double             | &check;      |
| stageVariableOverrides | Map<String,String> | &check;      |
| useStageCache          | Boolean            | &check;      |

#### MethodSetting
| **Name**                               | **Type** | **Nullable** |
| -------------------------------------- | -------- | ------------ |
| cacheDataEncrypted                     | Boolean  | &check;      |
| cacheTtlInSeconds                      | Int      | &check;      |
| cachingEnabled                         | Boolean  | &check;      |
| dataTraceEnabled                       | Boolean  | &check;      |
| loggingLevel                           | String   | &check;      |
| metricsEnabled                         | Boolean  | &check;      |
| requireAuthorizationForCacheControl    | Boolean  | &check;      |
| throttlingBurstLimit                   | Int      | &check;      |
| throttlingRateLimit                    | Double   | &check;      |
| unauthorizedCacheControlHeaderStrategy | String   | &check;      |
