---
description: Amazon Web Services VPC NAT Gateway
---
aws_vpc_nat_gateway
-------------------

| **Name**             | **Type**             | **Nullable** |
| -------------------- | -------------------- | ------------ |
| accountId            | String               | &cross;      |
| addresses            | List<Address>        | &cross;      |
| connectivityType     | String               | &check;      |
| createTime           | String               | &check;      |
| deleteTime           | String               | &check;      |
| failureCode          | String               | &check;      |
| failureMessage       | String               | &check;      |
| id                   | String               | &cross;      |
| provisionedBandwidth | ProvisionedBandwidth | &check;      |
| region               | String               | &cross;      |
| state                | String               | &check;      |
| subnetId             | String               | &check;      |
| tags                 | Map<String,String>   | &cross;      |
| vpcId                | String               | &check;      |

#### Address
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| allocationId       | String   | &check;      |
| networkInterfaceId | String   | &cross;      |
| privateIp          | String   | &check;      |
| publicIp           | String   | &check;      |

#### ProvisionedBandwidth
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| provisionTime | String   | &check;      |
| provisioned   | String   | &check;      |
| requestTime   | String   | &check;      |
| requested     | String   | &check;      |
| status        | String   | &check;      |
