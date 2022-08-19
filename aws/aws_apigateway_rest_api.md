---
description: Amazon Web Services ApiGateway Rest API
---
aws_apigateway_rest_api
-----------------------

| **Name**                  | **Type**              | **Nullable** |
| ------------------------- | --------------------- | ------------ |
| accountId                 | String                | &cross;      |
| accountName               | String                | &check;      |
| apiKeySource              | String                | &check;      |
| binaryMediaTypes          | List<String>          | &check;      |
| createdDate               | String                | &check;      |
| description               | String                | &check;      |
| disableExecuteApiEndpoint | Boolean               | &check;      |
| endpointConfiguration     | EndpointConfiguration | &check;      |
| id                        | String                | &cross;      |
| minimumCompressionSize    | Int                   | &check;      |
| name                      | String                | &check;      |
| policy                    | String                | &check;      |
| region                    | String                | &cross;      |
| tags                      | Map<String,String>    | &check;      |
| version                   | String                | &check;      |
| warnings                  | List<String>          | &check;      |

#### EndpointConfiguration
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| types          | List<String> | &check;      |
| vpcEndpointIds | List<String> | &check;      |
