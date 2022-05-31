---
description: MongoDB Atlas Network Peering Container
---
mongodb_network_peering_container
---------------------------------

| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| atlasCidrBlock      | String   | &check;      |
| azureSubscriptionId | String   | &check;      |
| gcpProjectId        | String   | &check;      |
| id                  | String   | &check;      |
| networkName         | String   | &check;      |
| project             | Project  | &cross;      |
| providerName        | String   | &check;      |
| provisioned         | Boolean  | &check;      |
| regionName          | String   | &check;      |
| vnetName            | String   | &check;      |
| vpcId               | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
