---
description: Amazon Web Services Route53 Hosted Zone
---
aws_route53_hosted_zone
-----------------------

| **Name**        | **Type**                | **Nullable** |
| --------------- | ----------------------- | ------------ |
| accountId       | String                  | &cross;      |
| accountName     | String                  | &check;      |
| callerReference | String                  | &check;      |
| id              | String                  | &cross;      |
| isPrivateZone   | Boolean                 | &cross;      |
| linkedService   | String                  | &check;      |
| name            | String                  | &cross;      |
| records         | List<ResourceRecordSet> | &check;      |

#### AliasTarget
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| dnsName              | String   | &check;      |
| evaluateTargetHealth | Boolean  | &check;      |
| hostedZoneId         | String   | &check;      |

#### GeoLocation
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| continentCode   | String   | &check;      |
| countryCode     | String   | &check;      |
| subdivisionCode | String   | &check;      |

#### ResourceRecordSet
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| aliasTarget             | AliasTarget  | &check;      |
| failover                | String       | &check;      |
| geoLocation             | GeoLocation  | &check;      |
| healthCheckId           | String       | &check;      |
| multiValueAnswer        | Boolean      | &check;      |
| name                    | String       | &cross;      |
| region                  | String       | &check;      |
| resourceRecords         | List<String> | &check;      |
| setIdentifier           | String       | &check;      |
| trafficPolicyInstanceId | String       | &check;      |
| ttl                     | Long         | &check;      |
| type                    | String       | &cross;      |
| weight                  | Long         | &check;      |
