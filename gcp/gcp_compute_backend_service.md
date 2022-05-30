---
description: Google Cloud Platform Compute Backend Service
---
gcp_compute_backend_service
---------------------------

| **Name**                 | **Type**                           | **Nullable** |
| ------------------------ | ---------------------------------- | ------------ |
| affinityCookieTtlSec     | Int                                | &check;      |
| backends                 | List<Backend>                      | &check;      |
| cdnPolicy                | CdnPolicy                          | &check;      |
| circuitBreakers          | CircuitBreakers                    | &check;      |
| connectionDraining       | ConnectionDraining                 | &check;      |
| connectionTrackingPolicy | ConnectionTrackingPolicy           | &check;      |
| consistentHash           | ConsistentHashLoadBalancerSettings | &check;      |
| creationTimestamp        | String                             | &check;      |
| customRequestHeaders     | List<String>                       | &check;      |
| customResponseHeaders    | List<String>                       | &check;      |
| description              | String                             | &check;      |
| edgeSecurityPolicy       | String                             | &check;      |
| enableCDN                | Boolean                            | &check;      |
| failoverPolicy           | FailoverPolicy                     | &check;      |
| healthChecks             | List<String>                       | &check;      |
| iap                      | IAP                                | &check;      |
| id                       | String                             | &cross;      |
| kind                     | String                             | &check;      |
| loadBalancingScheme      | String                             | &check;      |
| localityLbPolicy         | String                             | &check;      |
| logConfig                | BackendServiceLogConfig            | &check;      |
| maxStreamDuration        | String                             | &check;      |
| name                     | String                             | &check;      |
| network                  | String                             | &check;      |
| outlierDetection         | OutlierDetection                   | &check;      |
| port                     | Int                                | &check;      |
| portName                 | String                             | &check;      |
| project                  | String                             | &cross;      |
| protocol                 | String                             | &check;      |
| region                   | String                             | &check;      |
| securityPolicy           | String                             | &check;      |
| securitySettings         | SecuritySettings                   | &check;      |
| sessionAffinity          | String                             | &check;      |
| subsetting               | Subsetting                         | &check;      |
| timeoutSec               | Int                                | &check;      |

#### Backend
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| balancingMode             | String   | &check;      |
| capacityScaler            | Number   | &check;      |
| description               | String   | &check;      |
| failover                  | Boolean  | &check;      |
| group                     | String   | &check;      |
| maxConnections            | Int      | &check;      |
| maxConnectionsPerEndpoint | Int      | &check;      |
| maxConnectionsPerInstance | Int      | &check;      |
| maxRate                   | Int      | &check;      |
| maxRatePerEndpoint        | Number   | &check;      |
| maxRatePerInstance        | Number   | &check;      |
| maxUtilization            | Number   | &check;      |

#### BackendServiceLogConfig
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| enable     | Boolean  | &check;      |
| sampleRate | Number   | &check;      |

#### CdnPolicy
| **Name**                    | **Type**                                                     | **Nullable** |
| --------------------------- | ------------------------------------------------------------ | ------------ |
| bypassCacheOnRequestHeaders | List<CdnPolicy.BypassCacheOnRequestHeader>                   | &check;      |
| cacheKeyPolicy              | CdnPolicy.CacheKeyPolicy                                     | &check;      |
| cacheMode                   | String                                                       | &check;      |
| clientTtl                   | Int                                                          | &check;      |
| defaultTtl                  | Int                                                          | &check;      |
| maxTtl                      | Int                                                          | &check;      |
| negativeCaching             | Boolean                                                      | &check;      |
| negativeCachingPolicy       | List<CdnPolicy.BackendServiceCdnPolicyNegativeCachingPolicy> | &check;      |
| requestCoalescing           | Boolean                                                      | &check;      |
| serveWhileStale             | Int                                                          | &check;      |
| signedUrlCacheMaxAgeSec     | Long                                                         | &check;      |
| signedUrlKeyNames           | List<String>                                                 | &check;      |

#### CdnPolicy.BackendServiceCdnPolicyNegativeCachingPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | Int      | &check;      |
| ttl      | Int      | &check;      |

#### CdnPolicy.BypassCacheOnRequestHeader
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| headerName | String   | &check;      |

#### CdnPolicy.CacheKeyPolicy
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| includeHost          | Boolean      | &check;      |
| includeHttpHeaders   | List<String> | &check;      |
| includeNamedCookies  | List<String> | &check;      |
| includeProtocol      | Boolean      | &check;      |
| includeQueryString   | Boolean      | &check;      |
| queryStringBlacklist | List<String> | &check;      |
| queryStringWhitelist | List<String> | &check;      |

#### CircuitBreakers
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| maxConnections           | Int      | &check;      |
| maxPendingRequests       | Int      | &check;      |
| maxRequests              | Int      | &check;      |
| maxRequestsPerConnection | Int      | &check;      |
| maxRetries               | Int      | &check;      |

#### ConnectionDraining
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| drainingTimeoutSec | Int      | &check;      |

#### ConnectionTrackingPolicy
| **Name**                                 | **Type** | **Nullable** |
| ---------------------------------------- | -------- | ------------ |
| connectionPersistenceOnUnhealthyBackends | String   | &check;      |
| enableStrongAffinity                     | Boolean  | &check;      |
| idleTimeoutSec                           | Int      | &check;      |
| trackingMode                             | String   | &check;      |

#### ConsistentHashLoadBalancerSettings
| **Name**        | **Type**                                                                        | **Nullable** |
| --------------- | ------------------------------------------------------------------------------- | ------------ |
| httpCookie      | ConsistentHashLoadBalancerSettings.ConsistentHashLoadBalancerSettingsHttpCookie | &check;      |
| httpHeaderName  | String                                                                          | &check;      |
| minimumRingSize | Long                                                                            | &check;      |

#### ConsistentHashLoadBalancerSettings.ConsistentHashLoadBalancerSettingsHttpCookie
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| path     | String   | &check;      |
| ttl      | String   | &check;      |

#### FailoverPolicy
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| disableConnectionDrainOnFailover | Boolean  | &check;      |
| dropTrafficIfUnhealthy           | Boolean  | &check;      |
| failoverRatio                    | Number   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### IAP
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| enabled                  | Boolean  | &check;      |
| oauth2ClientId           | String   | &check;      |
| oauth2ClientSecret       | String   | &check;      |
| oauth2ClientSecretSha256 | String   | &check;      |

#### OutlierDetection
| **Name**                           | **Type** | **Nullable** |
| ---------------------------------- | -------- | ------------ |
| baseEjectionTime                   | String   | &check;      |
| consecutiveErrors                  | Int      | &check;      |
| consecutiveGatewayFailure          | Int      | &check;      |
| enforcingConsecutiveErrors         | Int      | &check;      |
| enforcingConsecutiveGatewayFailure | Int      | &check;      |
| enforcingSuccessRate               | Int      | &check;      |
| interval                           | String   | &check;      |
| maxEjectionPercent                 | Int      | &check;      |
| successRateMinimumHosts            | Int      | &check;      |
| successRateRequestVolume           | Int      | &check;      |
| successRateStdevFactor             | Int      | &check;      |

#### SecuritySettings
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| clientTlsPolicy | String       | &check;      |
| subjectAltNames | List<String> | &check;      |

#### Subsetting
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| policy   | String   | &check;      |
