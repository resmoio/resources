---
description: Google Workspace Building
---
gsuite_resource_building
------------------------

| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| address      | Address      | &check;      |
| buildingId   | String       | &cross;      |
| buildingName | String       | &check;      |
| coordinates  | Coordinates  | &check;      |
| customerId   | String       | &cross;      |
| description  | String       | &check;      |
| floorNames   | List<String> | &check;      |

#### Address
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| addressLines       | List<String> | &check;      |
| administrativeArea | String       | &check;      |
| languageCode       | String       | &check;      |
| locality           | String       | &check;      |
| postalCode         | String       | &check;      |
| regionCode         | String       | &check;      |
| sublocality        | String       | &check;      |

#### Coordinates
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| latitude  | Double   | &check;      |
| longitude | Double   | &check;      |
