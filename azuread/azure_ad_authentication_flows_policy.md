---
description: Azure Active Directory Authentication Flows Policy
---
azure_ad_authentication_flows_policy
------------------------------------

| **Name**          | **Type**                                         | **Nullable** |
| ----------------- | ------------------------------------------------ | ------------ |
| description       | String                                           | &check;      |
| displayName       | String                                           | &check;      |
| id                | String                                           | &cross;      |
| oDataType         | String                                           | &check;      |
| selfServiceSignUp | SelfServiceSignUpAuthenticationFlowConfiguration | &check;      |

#### SelfServiceSignUpAuthenticationFlowConfiguration
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| isEnabled | Boolean  | &check;      |
| oDataType | String   | &check;      |
