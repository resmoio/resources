---
description: Google Cloud Platform AppEngine Application
---
gcp_appengine_application
-------------------------

| **Name**                | **Type**              | **Nullable** |
| ----------------------- | --------------------- | ------------ |
| authDomain              | String                | &check;      |
| codeBucket              | String                | &check;      |
| databaseType            | String                | &check;      |
| defaultBucket           | String                | &check;      |
| defaultCookieExpiration | String                | &check;      |
| defaultHostname         | String                | &check;      |
| dispatchRules           | List<UrlDispatchRule> | &check;      |
| featureSettings         | FeatureSettings       | &check;      |
| gcrDomain               | String                | &check;      |
| iap                     | IdentityAwareProxy    | &check;      |
| id                      | String                | &cross;      |
| locationId              | String                | &check;      |
| name                    | String                | &cross;      |
| project                 | String                | &cross;      |
| servingStatus           | String                | &check;      |

#### FeatureSettings
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| splitHealthChecks       | Boolean  | &check;      |
| useContainerOptimizedOs | Boolean  | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### IdentityAwareProxy
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| enabled                  | Boolean  | &check;      |
| oauth2ClientId           | String   | &check;      |
| oauth2ClientSecret       | String   | &check;      |
| oauth2ClientSecretSha256 | String   | &check;      |

#### UrlDispatchRule
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &check;      |
| path     | String   | &check;      |
| service  | String   | &check;      |
