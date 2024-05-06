---
description: Okta Application
---
okta_application
----------------

| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| accessibility | Accessibility | &check;      |
| created       | String        | &check;      |
| features      | List<String>  | &check;      |
| id            | String        | &cross;      |
| label         | String        | &check;      |
| lastUpdated   | String        | &check;      |
| signOnMode    | String        | &check;      |
| status        | String        | &check;      |
| visibility    | Visibility    | &check;      |

#### Accessibility
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| errorRedirectUrl | String   | &check;      |
| loginRedirectUrl | String   | &check;      |
| selfService      | Boolean  | &check;      |

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
