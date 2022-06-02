---
description: Okta Policy Mapped Application
---
okta_policy_mapped_application
------------------------------

| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| accessibility | Accessibility | &check;      |
| created       | String        | &check;      |
| features      | List<String>  | &check;      |
| id            | String        | &cross;      |
| label         | String        | &check;      |
| lastUpdated   | String        | &check;      |
| name          | String        | &check;      |
| policyId      | String        | &cross;      |
| settings      | JSON          | &check;      |
| signOnMode    | String        | &check;      |
| status        | String        | &check;      |
| visibility    | Visibility    | &check;      |

#### Accessibility
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| errorRedirectUrl | String   | &check;      |
| loginRedirectUrl | String   | &check;      |
| selService       | Boolean  | &check;      |

#### Visibility
| **Name**          | **Type**        | **Nullable** |
| ----------------- | --------------- | ------------ |
| appLinks          | JSON            | &check;      |
| autoLaunch        | Boolean         | &check;      |
| autoSubmitToolbar | Boolean         | &check;      |
| hide              | Visibility.Hide | &check;      |

#### Visibility.Hide
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| iOS      | Boolean  | &check;      |
| web      | Boolean  | &check;      |
