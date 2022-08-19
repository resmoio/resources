---
description: Amazon Web Services EventBridge Connection
---
aws_eventbridge_connection
--------------------------

| **Name**           | **Type**                         | **Nullable** |
| ------------------ | -------------------------------- | ------------ |
| accountId          | String                           | &cross;      |
| accountName        | String                           | &check;      |
| arn                | String                           | &cross;      |
| authParameters     | ConnectionAuthResponseParameters | &check;      |
| authorizationType  | String                           | &cross;      |
| creationTime       | String                           | &check;      |
| description        | String                           | &check;      |
| lastAuthorizedTime | String                           | &check;      |
| lastModifiedTime   | String                           | &check;      |
| name               | String                           | &cross;      |
| region             | String                           | &cross;      |
| secretArn          | String                           | &check;      |
| state              | String                           | &cross;      |
| stateReason        | String                           | &check;      |

#### ConnectionAuthResponseParameters
| **Name**                 | **Type**                                                                | **Nullable** |
| ------------------------ | ----------------------------------------------------------------------- | ------------ |
| apiKeyAuthParameters     | ConnectionAuthResponseParameters.ConnectionApiKeyAuthResponseParameters | &check;      |
| basicAuthParameters      | ConnectionAuthResponseParameters.ConnectionBasicAuthResponseParameters  | &check;      |
| invocationHttpParameters | ConnectionAuthResponseParameters.ConnectionHttpParameters               | &check;      |
| oAuthParameters          | ConnectionAuthResponseParameters.ConnectionOAuthResponseParameters      | &check;      |

#### ConnectionAuthResponseParameters.ConnectionApiKeyAuthResponseParameters
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| apiKeyName | String   | &cross;      |

#### ConnectionAuthResponseParameters.ConnectionBasicAuthResponseParameters
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| username | String   | &cross;      |

#### ConnectionAuthResponseParameters.ConnectionHttpParameters
| **Name**              | **Type**                                                                            | **Nullable** |
| --------------------- | ----------------------------------------------------------------------------------- | ------------ |
| bodyParameters        | List<ConnectionAuthResponseParameters.ConnectionHttpParameters.ConnectionParameter> | &check;      |
| headerParameters      | List<ConnectionAuthResponseParameters.ConnectionHttpParameters.ConnectionParameter> | &check;      |
| queryStringParameters | List<ConnectionAuthResponseParameters.ConnectionHttpParameters.ConnectionParameter> | &check;      |

#### ConnectionAuthResponseParameters.ConnectionHttpParameters.ConnectionParameter
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| isValueSecret | Boolean  | &check;      |
| key           | String   | &cross;      |
| value         | String   | &check;      |

#### ConnectionAuthResponseParameters.ConnectionOAuthResponseParameters
| **Name**              | **Type**                                                                                                   | **Nullable** |
| --------------------- | ---------------------------------------------------------------------------------------------------------- | ------------ |
| authorizationEndpoint | String                                                                                                     | &cross;      |
| clientParameters      | ConnectionAuthResponseParameters.ConnectionOAuthResponseParameters.ConnectionOAuthClientResponseParameters | &check;      |
| httpMethod            | String                                                                                                     | &cross;      |
| oAuthHttpParameters   | ConnectionAuthResponseParameters.ConnectionHttpParameters                                                  | &check;      |

#### ConnectionAuthResponseParameters.ConnectionOAuthResponseParameters.ConnectionOAuthClientResponseParameters
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| clientID | String   | &cross;      |
