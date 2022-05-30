---
description: Amazon Web Services Elastic IP
---
aws_eip
-------

| **Name**                | **Type**           | **Nullable** |
| ----------------------- | ------------------ | ------------ |
| accountId               | String             | &cross;      |
| allocationId            | String             | &cross;      |
| associationId           | String             | &check;      |
| carrierIp               | String             | &check;      |
| customerOwnedIp         | String             | &check;      |
| customerOwnedIpv4Pool   | String             | &check;      |
| domain                  | String             | &check;      |
| instanceId              | String             | &check;      |
| networkBorderGroup      | String             | &check;      |
| networkInterfaceId      | String             | &check;      |
| networkInterfaceOwnerId | String             | &check;      |
| privateIpAddress        | String             | &check;      |
| publicIp                | String             | &check;      |
| publicIpv4Pool          | String             | &check;      |
| region                  | String             | &cross;      |
| tags                    | Map<String,String> | &check;      |
