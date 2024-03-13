---
description: Okta Network Zone
---
okta_network_zone
-----------------

| **Name**    | **Type**                 | **Nullable** |
| ----------- | ------------------------ | ------------ |
| created     | String                   | &check;      |
| gateways    | List<NetworkZoneAddress> | &check;      |
| id          | String                   | &cross;      |
| lastUpdated | String                   | &check;      |
| name        | String                   | &check;      |
| proxies     | List<NetworkZoneAddress> | &check;      |
| status      | String                   | &check;      |
| system      | Boolean                  | &check;      |
| type        | String                   | &check;      |
| usage       | String                   | &check;      |

#### NetworkZoneAddress
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| value    | String   | &check;      |
