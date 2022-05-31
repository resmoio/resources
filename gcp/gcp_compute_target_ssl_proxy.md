---
description: Google Cloud Platform Compute Target SSLProxy
---
gcp_compute_target_ssl_proxy
----------------------------

| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| creationTimestamp | String       | &check;      |
| description       | String       | &check;      |
| id                | String       | &cross;      |
| kind              | String       | &check;      |
| name              | String       | &check;      |
| project           | String       | &cross;      |
| proxyHeader       | String       | &check;      |
| service           | String       | &check;      |
| sslCertificates   | List<String> | &check;      |
| sslPolicy         | String       | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |
