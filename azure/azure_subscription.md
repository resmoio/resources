---
description: Azure Subscription
---
azure_subscription
------------------

| **Name**             | **Type**             | **Nullable** |
| -------------------- | -------------------- | ------------ |
| authorizationSource  | String               | &check;      |
| displayName          | String               | &cross;      |
| id                   | String               | &cross;      |
| locations            | List<Location>       | &check;      |
| managedByTenants     | List<String>         | &check;      |
| state                | String               | &cross;      |
| subscriptionId       | String               | &cross;      |
| subscriptionPolicies | SubscriptionPolicies | &check;      |
| tags                 | Map<String,String>   | &check;      |
| tenantId             | String               | &cross;      |

#### Location
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| displayName      | String   | &check;      |
| geographyGroup   | String   | &check;      |
| latitude         | String   | &check;      |
| longitude        | String   | &check;      |
| physicalLocation | String   | &check;      |
| region           | String   | &check;      |
| regionCategory   | String   | &check;      |
| regionType       | String   | &check;      |
| subscriptionId   | String   | &check;      |

#### SubscriptionPolicies
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| locationPlacementId | String   | &check;      |
| quotaId             | String   | &check;      |
| spendingLimit       | String   | &check;      |
