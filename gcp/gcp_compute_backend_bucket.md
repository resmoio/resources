---
description: Google Cloud Platform Compute Backend Bucket
---
gcp_compute_backend_bucket
--------------------------

| **Name**              | **Type**               | **Nullable** |
| --------------------- | ---------------------- | ------------ |
| bucketName            | String                 | &check;      |
| cdnPolicy             | BackendBucketCdnPolicy | &check;      |
| creationTimestamp     | String                 | &check;      |
| customResponseHeaders | List<String>           | &check;      |
| description           | String                 | &check;      |
| edgeSecurityPolicy    | String                 | &check;      |
| enableCdn             | Boolean                | &check;      |
| id                    | String                 | &cross;      |
| kind                  | String                 | &cross;      |
| name                  | String                 | &check;      |
| project               | String                 | &cross;      |

#### BackendBucketCdnPolicy
| **Name**                    | **Type**                                           | **Nullable** |
| --------------------------- | -------------------------------------------------- | ------------ |
| bypassCacheOnRequestHeaders | List<BackendBucketCdnPolicy.RequestHeader>         | &check;      |
| cacheKeyPolicy              | List<BackendBucketCdnPolicy.CacheKeyPolicy>        | &check;      |
| cacheMode                   | String                                             | &check;      |
| clientTtl                   | Int                                                | &check;      |
| defaultTtl                  | Int                                                | &check;      |
| maxTtl                      | Int                                                | &check;      |
| negativeCaching             | Boolean                                            | &check;      |
| negativeCachingPolicy       | List<BackendBucketCdnPolicy.NegativeCachingPolicy> | &check;      |
| requestCoalescing           | Boolean                                            | &check;      |
| serveWhileStale             | Int                                                | &check;      |
| signedUrlCacheMaxAgeSec     | Long                                               | &check;      |
| signedUrlKeyNames           | List<String>                                       | &check;      |

#### BackendBucketCdnPolicy.CacheKeyPolicy
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| includeHttpHeaders   | List<String> | &check;      |
| queryStringWhitelist | List<String> | &check;      |

#### BackendBucketCdnPolicy.NegativeCachingPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | Int      | &check;      |
| ttl      | Int      | &check;      |

#### BackendBucketCdnPolicy.RequestHeader
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| headerName | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
