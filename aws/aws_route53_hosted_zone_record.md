---
description: Amazon Web Services Route53 Hosted Zone Record
---
aws_route53_hosted_zone_record
------------------------------

| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| accountId               | String       | &cross;      |
| accountName             | String       | &check;      |
| aliasTarget             | AliasTarget  | &check;      |
| failover                | String       | &check;      |
| geoLocation             | GeoLocation  | &check;      |
| healthCheckId           | String       | &check;      |
| hostedZoneId            | String       | &cross;      |
| hostedZoneName          | String       | &cross;      |
| multiValueAnswer        | Boolean      | &check;      |
| name                    | String       | &cross;      |
| region                  | String       | &check;      |
| resourceRecords         | List<String> | &check;      |
| setIdentifier           | String       | &check;      |
| trafficPolicyInstanceId | String       | &check;      |
| ttl                     | Long         | &check;      |
| type                    | String       | &cross;      |
| weight                  | Long         | &check;      |

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
