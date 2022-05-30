---
description: Amazon Web Services OpenSearch Outbound Connection
---
aws_opensearch_outbound_connection
----------------------------------

| **Name**         | **Type**                   | **Nullable** |
| ---------------- | -------------------------- | ------------ |
| accountId        | String                     | &cross;      |
| alias            | String                     | &cross;      |
| id               | String                     | &cross;      |
| localDomainInfo  | DomainInformationContainer | &cross;      |
| region           | String                     | &cross;      |
| remoteDomainInfo | DomainInformationContainer | &cross;      |
| status           | OutboundConnectionStatus   | &cross;      |

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

#### OutboundConnectionStatus
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| message    | String   | &cross;      |
| statusCode | String   | &cross;      |
