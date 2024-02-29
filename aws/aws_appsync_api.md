---
description: Amazon Web Services AppSync API
---
aws_appsync_api
---------------

| **Name**                          | **Type**                               | **Nullable** |
| --------------------------------- | -------------------------------------- | ------------ |
| accountId                         | String                                 | &cross;      |
| accountName                       | String                                 | &check;      |
| additionalAuthenticationProviders | List<AdditionalAuthenticationProvider> | &check;      |
| apiId                             | String                                 | &cross;      |
| apiType                           | String                                 | &check;      |
| arn                               | String                                 | &check;      |
| authenticationType                | String                                 | &check;      |
| dns                               | Map<String,String>                     | &check;      |
| lambdaAuthorizerConfig            | LambdaAuthorizerConfig                 | &check;      |
| logConfig                         | LogConfig                              | &check;      |
| mergedApiExecutionRoleArn         | String                                 | &check;      |
| name                              | String                                 | &check;      |
| openIDConnectConfig               | OpenIDConnectConfig                    | &check;      |
| owner                             | String                                 | &check;      |
| ownerContact                      | String                                 | &check;      |
| region                            | String                                 | &cross;      |
| tags                              | Map<String,String>                     | &check;      |
| uris                              | Map<String,String>                     | &check;      |
| userPoolConfig                    | UserPoolConfig                         | &check;      |
| visibility                        | String                                 | &check;      |
| wafWebAclArn                      | String                                 | &check;      |
| xrayEnabled                       | Boolean                                | &check;      |

#### AdditionalAuthenticationProvider
| **Name**               | **Type**               | **Nullable** |
| ---------------------- | ---------------------- | ------------ |
| authenticationType     | String                 | &check;      |
| lambdaAuthorizerConfig | LambdaAuthorizerConfig | &check;      |
| openIDConnectConfig    | OpenIDConnectConfig    | &check;      |
| userPoolConfig         | CognitoUserPoolConfig  | &check;      |

#### CognitoUserPoolConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| appIdClientRegex | String   | &check;      |
| awsRegion        | String   | &check;      |
| userPoolId       | String   | &check;      |

#### LambdaAuthorizerConfig
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| authorizerResultTtlInSeconds | Int      | &check;      |
| authorizerUri                | String   | &check;      |
| identityValidationExpression | String   | &check;      |

#### LogConfig
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| cloudWatchLogsRoleArn | String   | &check;      |
| excludeVerboseContent | Boolean  | &check;      |
| fieldLogLevel         | String   | &check;      |

#### OpenIDConnectConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| authTTL  | Long     | &check;      |
| clientId | String   | &check;      |
| iatTTL   | Long     | &check;      |
| issuer   | String   | &check;      |

#### UserPoolConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| appIdClientRegex | String   | &check;      |
| awsRegion        | String   | &check;      |
| defaultAction    | String   | &check;      |
| userPoolId       | String   | &check;      |
