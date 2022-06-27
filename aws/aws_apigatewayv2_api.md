---
description: Amazon Web Services ApiGatewayV2 API
---
aws_apigatewayv2_api
--------------------

| **Name**                  | **Type**           | **Nullable** |
| ------------------------- | ------------------ | ------------ |
| accountId                 | String             | &cross;      |
| apiEndpoint               | String             | &check;      |
| apiGatewayManaged         | Boolean            | &check;      |
| apiId                     | String             | &cross;      |
| apiKeySelectionExpression | String             | &check;      |
| corsConfiguration         | Cors               | &check;      |
| createdDate               | String             | &check;      |
| description               | String             | &check;      |
| disableExecuteApiEndpoint | Boolean            | &check;      |
| disableSchemaValidation   | Boolean            | &check;      |
| importInfo                | List<String>       | &check;      |
| name                      | String             | &check;      |
| protocolType              | String             | &check;      |
| region                    | String             | &cross;      |
| routeSelectionExpression  | String             | &check;      |
| tags                      | Map<String,String> | &check;      |
| version                   | String             | &check;      |
| warnings                  | List<String>       | &check;      |

#### Cors
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| allowCredentials | Boolean      | &check;      |
| allowHeaders     | List<String> | &check;      |
| allowMethods     | List<String> | &check;      |
| allowOrigins     | List<String> | &check;      |
| exposeHeaders    | List<String> | &check;      |
| maxAge           | Int          | &check;      |
