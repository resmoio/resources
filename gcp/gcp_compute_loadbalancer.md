---
description: Google Cloud Platform Compute LoadBalancer
---
gcp_compute_loadbalancer
------------------------

| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| creationTimestamp  | String             | &check;      |
| defaultRouteAction | HttpRouteAction    | &check;      |
| defaultService     | String             | &check;      |
| defaultUrlRedirect | HttpRedirectAction | &check;      |
| description        | String             | &check;      |
| headerAction       | HttpHeaderAction   | &check;      |
| hostRules          | List<HostRule>     | &check;      |
| id                 | String             | &cross;      |
| kind               | String             | &check;      |
| name               | String             | &check;      |
| pathMatchers       | List<PathMatcher>  | &check;      |
| project            | String             | &cross;      |
| region             | String             | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### HostRule
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| description | String       | &check;      |
| hosts       | List<String> | &check;      |
| pathMatcher | String       | &check;      |

#### HttpHeaderAction
| **Name**                | **Type**                                | **Nullable** |
| ----------------------- | --------------------------------------- | ------------ |
| requestHeadersToAdd     | List<HttpHeaderAction.HttpHeaderOption> | &check;      |
| requestHeadersToRemove  | List<String>                            | &check;      |
| responseHeadersToAdd    | List<HttpHeaderAction.HttpHeaderOption> | &check;      |
| responseHeadersToRemove | List<String>                            | &check;      |

#### HttpHeaderAction.HttpHeaderOption
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| headerName  | String   | &check;      |
| headerValue | String   | &check;      |
| replace     | Boolean  | &check;      |

#### HttpRedirectAction
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| hostRedirect         | String   | &check;      |
| httpsRedirect        | Boolean  | &check;      |
| pathRedirect         | String   | &check;      |
| prefixRedirect       | String   | &check;      |
| redirectResponseCode | String   | &check;      |
| stripQuery           | Boolean  | &check;      |

#### HttpRouteAction
| **Name**                | **Type**                                     | **Nullable** |
| ----------------------- | -------------------------------------------- | ------------ |
| corsPolicy              | HttpRouteAction.CorsPolicy                   | &check;      |
| faultInjectionPolicy    | HttpRouteAction.HttpFaultInjection           | &check;      |
| maxStreamDuration       | String                                       | &check;      |
| requestMirrorPolicy     | HttpRouteAction.RequestMirrorPolicy          | &check;      |
| retryPolicy             | HttpRouteAction.HttpRetryPolicy              | &check;      |
| timeout                 | String                                       | &check;      |
| urlRewrite              | HttpRouteAction.UrlRewrite                   | &check;      |
| weightedBackendServices | List<HttpRouteAction.WeightedBackendService> | &check;      |

#### HttpRouteAction.CorsPolicy
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| allowCredentials   | Boolean      | &check;      |
| allowHeaders       | List<String> | &check;      |
| allowMethods       | List<String> | &check;      |
| allowOriginRegexes | List<String> | &check;      |
| allowOrigins       | List<String> | &check;      |
| disabled           | Boolean      | &check;      |
| exposeHeaders      | List<String> | &check;      |
| maxAge             | Int          | &check;      |

#### HttpRouteAction.HttpFaultInjection
| **Name** | **Type**                                          | **Nullable** |
| -------- | ------------------------------------------------- | ------------ |
| abort    | HttpRouteAction.HttpFaultInjection.HttpFaultAbort | &check;      |
| delay    | HttpRouteAction.HttpFaultInjection.HttpFaultDelay | &check;      |

#### HttpRouteAction.HttpFaultInjection.HttpFaultAbort
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| httpStatus | Int      | &check;      |
| percentage | Number   | &check;      |

#### HttpRouteAction.HttpFaultInjection.HttpFaultDelay
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| fixedDelay | String   | &check;      |
| percentage | Number   | &check;      |

#### HttpRouteAction.HttpRetryPolicy
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| numRetries      | Int          | &check;      |
| perTryTimeout   | String       | &check;      |
| retryConditions | List<String> | &check;      |

#### HttpRouteAction.RequestMirrorPolicy
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| backendService | String   | &check;      |

#### HttpRouteAction.UrlRewrite
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| hostRewrite       | String   | &check;      |
| pathPrefixRewrite | String   | &check;      |

#### HttpRouteAction.WeightedBackendService
| **Name**       | **Type**         | **Nullable** |
| -------------- | ---------------- | ------------ |
| backendService | String           | &check;      |
| headerAction   | HttpHeaderAction | &check;      |
| weight         | Int              | &check;      |

#### HttpRouteRule
| **Name**     | **Type**           | **Nullable** |
| ------------ | ------------------ | ------------ |
| description  | String             | &check;      |
| headerAction | HttpHeaderAction   | &check;      |
| priority     | Int                | &check;      |
| routeAction  | HttpRouteAction    | &check;      |
| service      | String             | &check;      |
| urlRedirect  | HttpRedirectAction | &check;      |

#### PathMatcher
| **Name**           | **Type**            | **Nullable** |
| ------------------ | ------------------- | ------------ |
| defaultRouteAction | HttpRouteAction     | &check;      |
| defaultService     | String              | &check;      |
| defaultUrlRedirect | HttpRedirectAction  | &check;      |
| description        | String              | &check;      |
| headerAction       | HttpHeaderAction    | &check;      |
| name               | String              | &check;      |
| pathRules          | List<PathRule>      | &check;      |
| routeRules         | List<HttpRouteRule> | &check;      |

#### PathRule
| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| paths       | List<String>       | &check;      |
| routeAction | HttpRouteAction    | &check;      |
| service     | String             | &check;      |
| urlRedirect | HttpRedirectAction | &check;      |
