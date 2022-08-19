---
description: Heroku Addon
---
heroku_addon
------------

| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| actions       | List<Action>  | &check;      |
| addonService  | AddonService  | &check;      |
| app           | App           | &check;      |
| billedPrice   | BilledPrice   | &check;      |
| billingEntity | BillingEntity | &check;      |
| configVars    | List<String>  | &check;      |
| createdAt     | String        | &check;      |
| id            | String        | &cross;      |
| name          | String        | &check;      |
| plan          | Plan          | &check;      |
| providerId    | String        | &check;      |
| state         | String        | &check;      |
| updatedAt     | String        | &check;      |
| web_url       | String        | &check;      |

#### Action
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| action        | String   | &check;      |
| id            | String   | &check;      |
| label         | String   | &check;      |
| requiresOwner | Boolean  | &check;      |
| url           | String   | &check;      |

#### AddonService
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### App
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### BilledPrice
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| cents    | Int      | &check;      |
| contract | Boolean  | &check;      |
| unit     | String   | &check;      |

#### BillingEntity
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### Plan
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
