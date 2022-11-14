---
description: Amazon Web Services EC2 Transit Gateway
---
aws_ec2_transit_gateway
-----------------------

| **Name**          | **Type**              | **Nullable** |
| ----------------- | --------------------- | ------------ |
| accountId         | String                | &cross;      |
| accountName       | String                | &check;      |
| creationTime      | String                | &check;      |
| description       | String                | &check;      |
| options           | TransitGatewayOptions | &check;      |
| ownerId           | String                | &check;      |
| region            | String                | &cross;      |
| state             | String                | &check;      |
| tags              | Map<String,String>    | &check;      |
| transitGatewayArn | String                | &cross;      |
| transitGatewayId  | String                | &check;      |

#### TransitGatewayOptions
| **Name**                       | **Type**     | **Nullable** |
| ------------------------------ | ------------ | ------------ |
| amazonSideAsn                  | Long         | &check;      |
| associationDefaultRouteTableId | String       | &check;      |
| autoAcceptSharedAttachments    | String       | &check;      |
| defaultRouteTableAssociation   | String       | &check;      |
| defaultRouteTablePropagation   | String       | &check;      |
| dnsSupport                     | String       | &check;      |
| multicastSupport               | String       | &check;      |
| propagationDefaultRouteTableId | String       | &check;      |
| transitGatewayCidrBlocks       | List<String> | &check;      |
| vpnEcmpSupport                 | String       | &check;      |
