---
description: Google Cloud Platform PUB/SUB Subscription
---
gcp_pubsub_subscription
-----------------------

| **Name**                      | **Type**           | **Nullable** |
| ----------------------------- | ------------------ | ------------ |
| ackDeadlineSeconds            | Int                | &check;      |
| deadLetterPolicy              | DeadLetterPolicy   | &check;      |
| detached                      | Boolean            | &check;      |
| enableMessageOrdering         | Boolean            | &check;      |
| expirationPolicy              | ExpirationPolicy   | &check;      |
| filter                        | String             | &check;      |
| labels                        | Map<String,String> | &check;      |
| messageRetentionDuration      | String             | &check;      |
| name                          | String             | &cross;      |
| project                       | String             | &cross;      |
| pushConfig                    | PushConfig         | &check;      |
| retainAckedMessages           | Boolean            | &check;      |
| retryPolicy                   | RetryPolicy        | &check;      |
| topic                         | String             | &check;      |
| topicMessageRetentionDuration | String             | &check;      |

#### DeadLetterPolicy
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| deadLetterTopic     | String   | &check;      |
| maxDeliveryAttempts | String   | &check;      |

#### ExpirationPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| ttl      | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### PushConfig
| **Name**     | **Type**             | **Nullable** |
| ------------ | -------------------- | ------------ |
| attributes   | Map<String,String>   | &check;      |
| oidcToken    | PushConfig.OIDCToken | &check;      |
| pushEndpoint | String               | &check;      |

#### PushConfig.OIDCToken
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| audience            | String   | &check;      |
| serviceAccountEmail | String   | &check;      |

#### RetryPolicy
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| maximumBackoff | String   | &check;      |
| minimumBackoff | String   | &check;      |
