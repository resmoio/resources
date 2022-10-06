---
description: Amazon Web Services VPC Endpoint
---
aws_vpc_endpoint
----------------

| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| accountId           | String             | &cross;      |
| accountName         | String             | &check;      |
| creationTimestamp   | String             | &check;      |
| dnsEntries          | List<DnsEntry>     | &check;      |
| groups              | List<Group>        | &check;      |
| id                  | String             | &cross;      |
| networkInterfaceIds | List<String>       | &check;      |
| ownerId             | String             | &check;      |
| policyDocument      | JSON               | &check;      |
| privateDnsEnabled   | Boolean            | &check;      |
| region              | String             | &cross;      |
| requesterManaged    | Boolean            | &check;      |
| routeTableIds       | List<String>       | &check;      |
| serviceName         | String             | &check;      |
| state               | String             | &check;      |
| subnetIds           | List<String>       | &check;      |
| tags                | Map<String,String> | &check;      |
| type                | String             | &check;      |

#### DnsEntry
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| dnsName      | String   | &cross;      |
| hostedZoneId | String   | &cross;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |
