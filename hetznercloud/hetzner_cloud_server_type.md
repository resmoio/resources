---
description: Hetzner Cloud Server Type
---
hetzner_cloud_server_type
-------------------------

| **Name**         | **Type**    | **Nullable** |
| ---------------- | ----------- | ------------ |
| architecture     | String      | &check;      |
| cores            | Long        | &check;      |
| cpu_type         | String      | &check;      |
| deprecated       | Boolean     | &check;      |
| deprecation      | Deprecation | &check;      |
| description      | String      | &check;      |
| disk             | Long        | &check;      |
| id               | Long        | &cross;      |
| included_traffic | Long        | &check;      |
| memory           | Long        | &check;      |
| name             | String      | &check;      |
| prices           | List<Price> | &check;      |
| storage_type     | String      | &check;      |

#### Deprecation
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| announced         | String   | &check;      |
| unavailable_after | String   | &check;      |

#### Price
| **Name**      | **Type**           | **Nullable** |
| ------------- | ------------------ | ------------ |
| location      | String             | &check;      |
| price_hourly  | Price.PriceHourly  | &check;      |
| price_monthly | Price.PriceMonthly | &check;      |

#### Price.PriceHourly
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gross    | String   | &check;      |
| net      | String   | &check;      |

#### Price.PriceMonthly
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| gross    | String   | &check;      |
| net      | String   | &check;      |
