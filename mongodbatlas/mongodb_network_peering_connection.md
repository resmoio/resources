---
description: MongoDB Atlas Network Peering Connection
---
mongodb_network_peering_connection
----------------------------------

| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| accepterRegionName  | String   | &check;      |
| awsAccountId        | String   | &check;      |
| azureDirectoryId    | String   | &check;      |
| azureSubscriptionId | String   | &check;      |
| connectionId        | String   | &check;      |
| containerId         | String   | &check;      |
| errorState          | String   | &check;      |
| errorStateName      | String   | &check;      |
| gcpProjectId        | String   | &check;      |
| id                  | String   | &cross;      |
| networkName         | String   | &check;      |
| project             | Project  | &cross;      |
| resourceGroupName   | String   | &check;      |
| routeTableCidrBlock | String   | &check;      |
| status              | String   | &check;      |
| statusName          | String   | &check;      |
| vnetName            | String   | &check;      |
| vpcId               | String   | &check;      |

#### Project
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
