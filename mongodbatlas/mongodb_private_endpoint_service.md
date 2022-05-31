---
description: MongoDB Atlas Private Endpoint Service
---
mongodb_private_endpoint_service
--------------------------------

| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| endpointGroupNames           | List<String> | &check;      |
| endpointServiceName          | String       | &check;      |
| errorMessage                 | String       | &check;      |
| id                           | String       | &cross;      |
| interfaceEndpoints           | List<String> | &check;      |
| privateEndpoints             | List<String> | &check;      |
| privateLinkServiceName       | String       | &check;      |
| privateLinkServiceResourceId | String       | &check;      |
| project                      | Project      | &cross;      |
| provider                     | String       | &cross;      |
| regionName                   | String       | &check;      |
| serviceAttachmentNames       | List<String> | &check;      |
| status                       | String       | &check;      |

#### Link
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| href     | String   | &check;      |
| rel      | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
