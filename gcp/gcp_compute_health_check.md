---
description: Google Cloud Platform Compute Health Check
---
gcp_compute_health_check
------------------------

| **Name**           | **Type**             | **Nullable** |
| ------------------ | -------------------- | ------------ |
| checkIntervalSec   | Int                  | &check;      |
| creationTimestamp  | String               | &check;      |
| description        | String               | &check;      |
| grpcHealthCheck    | GRPCHealthCheck      | &check;      |
| healthyThreshold   | Int                  | &check;      |
| http2HealthCheck   | HTTP2HealthCheck     | &check;      |
| httpHealthCheck    | HTTPHealthCheck      | &check;      |
| httpsHealthCheck   | HTTPSHealthCheck     | &check;      |
| id                 | String               | &cross;      |
| kind               | String               | &check;      |
| logConfig          | HealthCheckLogConfig | &check;      |
| name               | String               | &check;      |
| project            | String               | &cross;      |
| region             | String               | &check;      |
| sslHealthCheck     | SSLHealthCheck       | &check;      |
| tcpHealthCheck     | TCPHealthCheck       | &check;      |
| timeoutSec         | Int                  | &check;      |
| type               | String               | &check;      |
| unhealthyThreshold | Int                  | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### GRPCHealthCheck
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| grpcServiceName   | String   | &check;      |
| port              | Int      | &check;      |
| portName          | String   | &check;      |
| portSpecification | String   | &check;      |

#### HTTP2HealthCheck
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| host              | String   | &check;      |
| port              | Int      | &check;      |
| portName          | String   | &check;      |
| portSpecification | String   | &check;      |
| proxyHeader       | String   | &check;      |
| requestPath       | String   | &check;      |
| response          | String   | &check;      |

#### HTTPHealthCheck
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| host              | String   | &check;      |
| port              | Int      | &check;      |
| portName          | String   | &check;      |
| portSpecification | String   | &check;      |
| proxyHeader       | String   | &check;      |
| requestPath       | String   | &check;      |
| response          | String   | &check;      |

#### HTTPSHealthCheck
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| host              | String   | &check;      |
| port              | Int      | &check;      |
| portName          | String   | &check;      |
| portSpecification | String   | &check;      |
| proxyHeader       | String   | &check;      |
| requestPath       | String   | &check;      |
| response          | String   | &check;      |

#### HealthCheckLogConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enable   | Boolean  | &check;      |

#### SSLHealthCheck
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| port              | Int      | &check;      |
| portName          | String   | &check;      |
| portSpecification | String   | &check;      |
| proxyHeader       | String   | &check;      |
| request           | String   | &check;      |
| response          | String   | &check;      |

#### TCPHealthCheck
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| port              | Int      | &check;      |
| portName          | String   | &check;      |
| portSpecification | String   | &check;      |
| proxyHeader       | String   | &check;      |
| request           | String   | &check;      |
| response          | String   | &check;      |
