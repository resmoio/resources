---
description: Google Cloud Platform Compute Target HttpsProxy
---
gcp_compute_target_https_proxy
------------------------------

| **Name**            | **Type**     | **Nullable** |
| ------------------- | ------------ | ------------ |
| authorizationPolicy | String       | &check;      |
| creationTimestamp   | String       | &check;      |
| description         | String       | &check;      |
| id                  | String       | &cross;      |
| kind                | String       | &check;      |
| name                | String       | &check;      |
| project             | String       | &cross;      |
| proxyBind           | Boolean      | &check;      |
| quicOverride        | String       | &check;      |
| region              | String       | &check;      |
| serverTlsPolicy     | String       | &check;      |
| sslCertificates     | List<String> | &check;      |
| sslPolicy           | String       | &check;      |
| urlMap              | String       | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
