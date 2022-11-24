---
description: Amazon Web Services VPC Subnet
---
aws_vpc_subnet
--------------

| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| accountId           | String             | &cross;      |
| accountName         | String             | &check;      |
| availabilityZoneId  | String             | &check;      |
| cidr                | String             | &check;      |
| defaultForAz        | Boolean            | &check;      |
| enableDns64         | Boolean            | &check;      |
| id                  | String             | &cross;      |
| ipv6Native          | Boolean            | &check;      |
| mapPublicIpOnLaunch | Boolean            | &check;      |
| region              | String             | &cross;      |
| state               | String             | &check;      |
| subnetArn           | String             | &check;      |
| tags                | Map<String,String> | &check;      |
| vpcId               | String             | &cross;      |
| zone                | String             | &cross;      |
