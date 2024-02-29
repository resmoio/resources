---
description: Amazon Web Services Access Analyzer Finding
---
aws_access_analyzer_finding
---------------------------

| **Name**             | **Type**            | **Nullable** |
| -------------------- | ------------------- | ------------ |
| accountId            | String              | &cross;      |
| accountName          | String              | &check;      |
| action               | List<String>        | &check;      |
| analyzedAt           | String              | &check;      |
| analyzerArn          | String              | &cross;      |
| analyzerName         | String              | &cross;      |
| condition            | Map<String,String>  | &check;      |
| createdAt            | String              | &check;      |
| error                | String              | &check;      |
| id                   | String              | &cross;      |
| isPublic             | Boolean             | &check;      |
| principal            | Map<String,String>  | &check;      |
| region               | String              | &cross;      |
| resource             | String              | &check;      |
| resourceOwnerAccount | String              | &check;      |
| resourceType         | String              | &check;      |
| sources              | List<FindingSource> | &check;      |
| status               | String              | &check;      |
| updatedAt            | String              | &check;      |

#### FindingSource
| **Name** | **Type**            | **Nullable** |
| -------- | ------------------- | ------------ |
| detail   | FindingSourceDetail | &check;      |
| type     | String              | &check;      |

#### FindingSourceDetail
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| accessPointAccount | String   | &check;      |
| accessPointArn     | String   | &check;      |
