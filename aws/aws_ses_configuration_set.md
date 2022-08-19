---
description: Amazon Web Services SES Configuration Set
---
aws_ses_configuration_set
-------------------------

| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| accountId            | String             | &cross;      |
| accountName          | String             | &check;      |
| configurationSetName | String             | &cross;      |
| deliveryOptions      | DeliveryOptions    | &check;      |
| region               | String             | &cross;      |
| reputationOptions    | ReputationOptions  | &check;      |
| sendingOptions       | SendingOptions     | &check;      |
| suppressionOptions   | SuppressionOptions | &check;      |
| tags                 | Map<String,String> | &check;      |
| trackingOptions      | TrackingOptions    | &check;      |

#### DeliveryOptions
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| sendingPoolName | String   | &check;      |
| tlsPolicy       | String   | &check;      |

#### ReputationOptions
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| lastFreshStart           | String   | &check;      |
| reputationMetricsEnabled | Boolean  | &check;      |

#### SendingOptions
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| sendingEnabled | Boolean  | &check;      |

#### SuppressionOptions
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| suppressedReasons | List<String> | &check;      |

#### TrackingOptions
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| customRedirectDomain | String   | &check;      |
