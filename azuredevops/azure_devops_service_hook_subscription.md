---
description: Azure DevOps Service Hook Subscription
---
azure_devops_service_hook_subscription
--------------------------------------

| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| accountId              | String   | &cross;      |
| accountName            | String   | &cross;      |
| actionDescription      | String   | &check;      |
| consumerActionId       | String   | &check;      |
| consumerId             | String   | &check;      |
| consumerInputs         | JSON     | &check;      |
| createdBy              | Identity | &check;      |
| createdDate            | String   | &check;      |
| eventDescription       | String   | &check;      |
| eventType              | String   | &check;      |
| id                     | String   | &cross;      |
| lastProbationRetryDate | String   | &check;      |
| modifiedBy             | Identity | &check;      |
| modifiedDate           | String   | &check;      |
| probationRetries       | String   | &check;      |
| publisherId            | String   | &check;      |
| publisherInputs        | JSON     | &check;      |
| resourceVersion        | String   | &check;      |
| status                 | String   | &check;      |
| subscriber             | Identity | &check;      |
| url                    | String   | &check;      |

#### Identity
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| displayName       | String   | &check;      |
| id                | String   | &check;      |
| imageUrl          | String   | &check;      |
| isAadIdentity     | Boolean  | &check;      |
| isContainer       | Boolean  | &check;      |
| isDeletedInOrigin | Boolean  | &check;      |
| profileUrl        | String   | &check;      |
| uniqueName        | String   | &check;      |
| url               | String   | &check;      |
