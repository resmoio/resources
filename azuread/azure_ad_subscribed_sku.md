---
description: Azure Active Directory Subscribed SKU
---
azure_ad_subscribed_sku
-----------------------

| **Name**         | **Type**              | **Nullable** |
| ---------------- | --------------------- | ------------ |
| accountId        | String                | &check;      |
| accountName      | String                | &check;      |
| appliesTo        | String                | &check;      |
| capabilityStatus | String                | &check;      |
| consumedUnits    | Int                   | &check;      |
| id               | String                | &cross;      |
| oDataType        | String                | &check;      |
| prepaidUnits     | LicenseUnitsDetail    | &check;      |
| servicePlans     | List<ServicePlanInfo> | &check;      |
| skuId            | String                | &check;      |
| skuPartNumber    | String                | &check;      |
| subscriptionIds  | List<String>          | &check;      |

#### LicenseUnitsDetail
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| enabled   | Int      | &check;      |
| oDataType | String   | &check;      |
| suspended | Int      | &check;      |
| warning   | Int      | &check;      |

#### ServicePlanInfo
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| appliesTo          | String   | &check;      |
| oDataType          | String   | &check;      |
| provisioningStatus | String   | &check;      |
| servicePlanId      | String   | &check;      |
| servicePlanName    | String   | &check;      |
