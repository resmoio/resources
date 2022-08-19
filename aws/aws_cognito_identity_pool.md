---
description: Amazon Web Services Cognito Identity Pool
---
aws_cognito_identity_pool
-------------------------

| **Name**                       | **Type**                      | **Nullable** |
| ------------------------------ | ----------------------------- | ------------ |
| accountId                      | String                        | &cross;      |
| accountName                    | String                        | &check;      |
| allowClassicFlow               | Boolean                       | &check;      |
| allowUnauthenticatedIdentities | Boolean                       | &check;      |
| cognitoIdentityProviders       | List<CognitoIdentityProvider> | &check;      |
| developerProviderName          | String                        | &check;      |
| identityPoolId                 | String                        | &cross;      |
| identityPoolName               | String                        | &check;      |
| identityPoolTags               | Map<String,String>            | &check;      |
| openIdConnectProviderARNs      | List<String>                  | &check;      |
| region                         | String                        | &cross;      |
| samlProviderARNs               | List<String>                  | &check;      |
| supportedLoginProviders        | Map<String,String>            | &check;      |

#### CognitoIdentityProvider
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| clientId             | String   | &check;      |
| providerName         | String   | &check;      |
| serverSideTokenCheck | Boolean  | &check;      |
