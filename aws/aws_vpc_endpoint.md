---
description: Amazon Web Services VPC Endpoint
---
aws_vpc_endpoint
----------------

| **Name**            | **Type**           | **Nullable** |
| ------------------- | ------------------ | ------------ |
| accountId           | String             | &cross;      |
| accountName         | String             | &check;      |
| creationTimestamp   | String             | &cross;      |
| dnsEntries          | List<DnsEntry>     | &cross;      |
| groups              | List<Group>        | &cross;      |
| id                  | String             | &cross;      |
| networkInterfaceIds | List<String>       | &cross;      |
| ownerId             | String             | &cross;      |
| policyDocument      | JSON               | &check;      |
| privateDnsEnabled   | Boolean            | &cross;      |
| region              | String             | &cross;      |
| requesterManaged    | Boolean            | &cross;      |
| routeTableIds       | List<String>       | &cross;      |
| serviceName         | String             | &cross;      |
| state               | String             | &cross;      |
| subnetIds           | List<String>       | &cross;      |
| tags                | Map<String,String> | &cross;      |
| type                | String             | &cross;      |

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
