---
description: Amazon Web Services OpenSearch Inbound Connection
---
aws_opensearch_inbound_connection
---------------------------------

| **Name**         | **Type**                   | **Nullable** |
| ---------------- | -------------------------- | ------------ |
| accountId        | String                     | &cross;      |
| id               | String                     | &cross;      |
| localDomainInfo  | DomainInformationContainer | &cross;      |
| region           | String                     | &cross;      |
| remoteDomainInfo | DomainInformationContainer | &cross;      |
| status           | InboundConnectionStatus    | &cross;      |

#### DomainInformationContainer
| **Name**             | **Type**                                        | **Nullable** |
| -------------------- | ----------------------------------------------- | ------------ |
| awsDomainInformation | DomainInformationContainer.AWSDomainInformation | &cross;      |

#### DomainInformationContainer.AWSDomainInformation
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| domainName | String   | &cross;      |
| ownerId    | String   | &cross;      |
| region     | String   | &cross;      |

#### InboundConnectionStatus
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| message    | String   | &cross;      |
| statusCode | String   | &cross;      |
