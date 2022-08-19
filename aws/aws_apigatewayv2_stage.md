---
description: Amazon Web Services ApiGatewayV2 Stage
---
aws_apigatewayv2_stage
----------------------

| **Name**                    | **Type**                  | **Nullable** |
| --------------------------- | ------------------------- | ------------ |
| accessLogSettings           | AccessLogSettings         | &check;      |
| accountId                   | String                    | &cross;      |
| accountName                 | String                    | &check;      |
| apiGatewayManaged           | Boolean                   | &check;      |
| apiId                       | String                    | &check;      |
| autoDeploy                  | Boolean                   | &check;      |
| clientCertificateId         | String                    | &check;      |
| createdDate                 | String                    | &check;      |
| defaultRouteSettings        | RouteSettings             | &check;      |
| deploymentId                | String                    | &check;      |
| description                 | String                    | &check;      |
| lastDeploymentStatusMessage | String                    | &check;      |
| lastUpdatedDate             | String                    | &check;      |
| region                      | String                    | &cross;      |
| routeSettings               | Map<String,RouteSettings> | &check;      |
| stageName                   | String                    | &cross;      |
| stageVariables              | Map<String,String>        | &check;      |
| tags                        | Map<String,String>        | &check;      |

#### AccessLogSettings
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| destinationArn | String   | &check;      |
| format         | String   | &check;      |

#### RouteSettings
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| dataTraceEnabled       | Boolean  | &check;      |
| detailedMetricsEnabled | Boolean  | &check;      |
| loggingLevel           | String   | &check;      |
| throttlingBurstLimit   | Int      | &check;      |
| throttlingRateLimit    | Double   | &check;      |
