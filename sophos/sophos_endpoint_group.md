---
description: Sophos Endpoint Group
---
sophos_endpoint_group
---------------------

| **Name**    | **Type**       | **Nullable** |
| ----------- | -------------- | ------------ |
| createdAt   | String         | &check;      |
| description | String         | &check;      |
| endpoints   | List<Endpoint> | &check;      |
| id          | String         | &cross;      |
| name        | String         | &cross;      |
| tenant      | Tenant         | &cross;      |
| type        | String         | &cross;      |
| updatedAt   | String         | &check;      |

#### Endpoint
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| items      | List<EndpointItem> | &check;      |
| itemsCount | Int                | &check;      |
| total      | Int                | &check;      |

#### EndpointItem
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| hostname | String   | &check;      |
| id       | String   | &check;      |

#### Tenant
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |
