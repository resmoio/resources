---
description: Google Cloud Platform DNS Policy
---
gcp_dns_policy
--------------

| **Name**                    | **Type**         | **Nullable** |
| --------------------------- | ---------------- | ------------ |
| alternativeNameServerConfig | NameServerConfig | &check;      |
| description                 | String           | &check;      |
| enableInboundForwarding     | Boolean          | &check;      |
| enableLogging               | Boolean          | &check;      |
| id                          | String           | &cross;      |
| name                        | String           | &check;      |
| networks                    | List<Network>    | &check;      |
| project                     | String           | &cross;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### NameServer
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| forwardingPath | String   | &check;      |
| ipv4Address    | String   | &check;      |
| kind           | String   | &check;      |

#### NameServerConfig
| **Name**          | **Type**         | **Nullable** |
| ----------------- | ---------------- | ------------ |
| kind              | String           | &check;      |
| targetNameServers | List<NameServer> | &check;      |

#### Network
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| kind       | String   | &check;      |
| networkUrl | String   | &check;      |
