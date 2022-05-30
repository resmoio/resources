---
description: Google Cloud Platform VPC Network
---
gcp_vpc_network
---------------

| **Name**              | **Type**             | **Nullable** |
| --------------------- | -------------------- | ------------ |
| autoCreateSubnetworks | Boolean              | &check;      |
| creationTimestamp     | String               | &check;      |
| description           | String               | &check;      |
| gatewayIPv4           | String               | &check;      |
| iPv4Range             | String               | &check;      |
| id                    | Long                 | &cross;      |
| kind                  | String               | &cross;      |
| mtu                   | Int                  | &check;      |
| name                  | String               | &check;      |
| peerings              | List<NetworkPeering> | &check;      |
| project               | String               | &cross;      |
| routingConfig         | NetworkRoutingConfig | &check;      |
| subnetworks           | List<String>         | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### NetworkPeering
| **Name**                       | **Type** | **Nullable** |
| ------------------------------ | -------- | ------------ |
| autoCreateRoutes               | Boolean  | &check;      |
| exchangeSubnetRoutes           | Boolean  | &check;      |
| exportCustomRoutes             | Boolean  | &check;      |
| exportSubnetRoutesWithPublicIp | Boolean  | &check;      |
| importCustomRoutes             | Boolean  | &check;      |
| importSubnetRoutesWithPublicIp | Boolean  | &check;      |
| name                           | String   | &check;      |
| network                        | String   | &check;      |
| peerMtu                        | Int      | &check;      |
| state                          | String   | &check;      |
| stateDetails                   | String   | &check;      |

#### NetworkRoutingConfig
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| routingMode | String   | &cross;      |
