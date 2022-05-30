---
description: Amazon Web Services ELB Target Group
---
aws_elb_target_group
--------------------

| **Name**                   | **Type**           | **Nullable** |
| -------------------------- | ------------------ | ------------ |
| accountId                  | String             | &cross;      |
| attributes                 | Map<String,String> | &check;      |
| healthCheckEnabled         | Boolean            | &check;      |
| healthCheckIntervalSeconds | Int                | &check;      |
| healthCheckPath            | String             | &check;      |
| healthCheckPort            | String             | &check;      |
| healthCheckProtocol        | String             | &check;      |
| healthCheckTimeoutSeconds  | Int                | &check;      |
| healthyThresholdCount      | Int                | &check;      |
| ipAddressType              | String             | &check;      |
| loadBalancerArns           | List<String>       | &check;      |
| matcher                    | Matcher            | &check;      |
| port                       | Int                | &check;      |
| protocolVersion            | String             | &check;      |
| region                     | String             | &cross;      |
| targetGroupArn             | String             | &cross;      |
| targetGroupName            | String             | &cross;      |
| targetType                 | String             | &check;      |
| unhealthyThresholdCount    | Int                | &check;      |
| vpcId                      | String             | &check;      |

#### Matcher
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| grpcCode | String   | &check;      |
| httpCode | String   | &check;      |
