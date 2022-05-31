---
description: Resmo Rule
---
resmo_rule
----------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| accountId    | String       | &check;      |
| createdAt    | Timestamp    | &check;      |
| createdBy    | String       | &check;      |
| description  | String       | &check;      |
| evaluation   | String       | &check;      |
| id           | String       | &cross;      |
| integrations | List<String> | &check;      |
| name         | String       | &check;      |
| queries      | List<Query>  | &check;      |
| remediation  | String       | &check;      |
| resources    | List<String> | &check;      |
| severity     | String       | &check;      |
| tags         | List<String> | &check;      |
| updatedAt    | Timestamp    | &check;      |

#### Query
| **Name** | **Type**  | **Nullable** |
| -------- | --------- | ------------ |
| label    | String    | &check;      |
| raw      | Query.Raw | &check;      |
| ref      | Query.Ref | &check;      |

#### Query.Raw
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| sql      | String   | &cross;      |

#### Query.Ref
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
