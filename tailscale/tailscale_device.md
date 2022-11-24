---
description: Tailscale Device
---
tailscale_device
----------------

| **Name**                  | **Type**           | **Nullable** |
| ------------------------- | ------------------ | ------------ |
| addresses                 | List<String>       | &check;      |
| advertisedRoutes          | List<String>       | &check;      |
| authorized                | Boolean            | &check;      |
| blocksIncomingConnections | Boolean            | &check;      |
| clientConnectivity        | ClientConnectivity | &check;      |
| clientVersion             | String             | &check;      |
| created                   | String             | &check;      |
| enabledRoutes             | List<String>       | &check;      |
| expires                   | String             | &check;      |
| hostname                  | String             | &check;      |
| id                        | String             | &cross;      |
| isExternal                | Boolean            | &check;      |
| keyExpiryDisabled         | Boolean            | &check;      |
| lastSeen                  | String             | &check;      |
| machineKey                | String             | &check;      |
| name                      | String             | &check;      |
| nodeId                    | String             | &check;      |
| nodeKey                   | String             | &check;      |
| os                        | String             | &check;      |
| updateAvailable           | Boolean            | &check;      |
| user                      | String             | &check;      |

#### ClientConnectivity
| **Name**              | **Type**            | **Nullable** |
| --------------------- | ------------------- | ------------ |
| clientSupports        | Map<String,Boolean> | &check;      |
| derp                  | String              | &check;      |
| endpoints             | List<String>        | &check;      |
| mappingVariesByDestIP | Boolean             | &check;      |
