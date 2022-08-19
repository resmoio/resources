---
description: Amazon Web Services VPC Route Table
---
aws_vpc_route_table
-------------------

| **Name**     | **Type**           | **Nullable** |
| ------------ | ------------------ | ------------ |
| accountId    | String             | &cross;      |
| accountName  | String             | &check;      |
| associations | List<Association>  | &cross;      |
| id           | String             | &cross;      |
| ownerId      | String             | &cross;      |
| region       | String             | &cross;      |
| routes       | List<Route>        | &cross;      |
| tags         | Map<String,String> | &cross;      |
| vpcId        | String             | &cross;      |

#### Association
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| main     | Boolean  | &cross;      |
| state    | String   | &cross;      |

#### Route
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| destinationCidrBlock        | String   | &check;      |
| destinationIpv6CidrBlock    | String   | &check;      |
| destinationPrefixListId     | String   | &check;      |
| egressOnlyInternetGatewayId | String   | &check;      |
| gatewayId                   | String   | &check;      |
| instanceId                  | String   | &check;      |
| networkInterfaceId          | String   | &check;      |
| origin                      | String   | &check;      |
| state                       | String   | &check;      |
| transitGatewayId            | String   | &check;      |
| vpcPeeringConnectionId      | String   | &check;      |
