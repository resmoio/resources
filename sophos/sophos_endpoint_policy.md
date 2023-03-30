---
description: Sophos Endpoint Policy
---
sophos_endpoint_policy
----------------------

| **Name**                | **Type**  | **Nullable** |
| ----------------------- | --------- | ------------ |
| appliesTo               | AppliesTo | &check;      |
| createdAt               | String    | &check;      |
| createdBy               | Actor     | &check;      |
| enabled                 | Boolean   | &cross;      |
| id                      | String    | &cross;      |
| lockedByManagingAccount | Boolean   | &check;      |
| name                    | String    | &cross;      |
| priority                | Int       | &check;      |
| settings                | JSON      | &check;      |
| tenant                  | Tenant    | &cross;      |
| type                    | String    | &cross;      |
| updatedAt               | String    | &check;      |
| updatedBy               | Actor     | &check;      |

#### Actor
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| accountId   | String   | &check;      |
| accountType | String   | &check;      |
| id          | String   | &cross;      |
| name        | String   | &check;      |
| type        | String   | &cross;      |

#### AppliesTo
| **Name**       | **Type**   | **Nullable** |
| -------------- | ---------- | ------------ |
| endpointGroups | List<JSON> | &check;      |
| endpoints      | List<JSON> | &check;      |
| userGroups     | List<JSON> | &check;      |
| users          | List<JSON> | &check;      |

#### Tenant
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
