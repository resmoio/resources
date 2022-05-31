---
description: PagerDuty Webhook Subscription
---
pagerduty_webhook_subscription
------------------------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| active         | Boolean        | &check;      |
| deliveryMethod | DeliveryMethod | &check;      |
| description    | String         | &check;      |
| events         | List<String>   | &cross;      |
| filter         | Filter         | &check;      |
| id             | String         | &cross;      |
| type           | String         | &check;      |

#### DeliveryMethod
| **Name**            | **Type**                          | **Nullable** |
| ------------------- | --------------------------------- | ------------ |
| customHeaders       | List<DeliveryMethod.CustomHeader> | &check;      |
| id                  | String                            | &check;      |
| temporarilyDisabled | Boolean                           | &cross;      |
| type                | String                            | &check;      |
| url                 | String                            | &check;      |

#### DeliveryMethod.CustomHeader
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### Filter
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| type     | String   | &check;      |
