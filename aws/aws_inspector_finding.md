---
description: Amazon Web Services Inspector Finding
---
aws_inspector_finding
---------------------

| **Name**              | **Type**                   | **Nullable** |
| --------------------- | -------------------------- | ------------ |
| accountId             | String                     | &cross;      |
| arn                   | String                     | &cross;      |
| assetAttributes       | AssetAttributes            | &check;      |
| assetType             | String                     | &check;      |
| attributes            | Map<String,String>         | &check;      |
| confidence            | Int                        | &check;      |
| createdAt             | String                     | &check;      |
| description           | String                     | &check;      |
| id                    | String                     | &check;      |
| indicatorOfCompromise | Boolean                    | &check;      |
| numericSeverity       | Double                     | &check;      |
| recommendation        | String                     | &check;      |
| schemaVersion         | Int                        | &check;      |
| service               | String                     | &check;      |
| serviceAttributes     | InspectorServiceAttributes | &check;      |
| severity              | String                     | &check;      |
| title                 | String                     | &check;      |
| updatedAt             | String                     | &check;      |
| userAttributes        | Map<String,String>         | &check;      |

#### AssetAttributes
| **Name**          | **Type**               | **Nullable** |
| ----------------- | ---------------------- | ------------ |
| agentId           | String                 | &check;      |
| amiId             | String                 | &check;      |
| autoScalingGroup  | String                 | &check;      |
| hostname          | String                 | &check;      |
| ipv4Addresses     | List<String>           | &check;      |
| networkInterfaces | List<NetworkInterface> | &check;      |
| schemaVersion     | Int                    | &check;      |
| tags              | Map<String,String>     | &check;      |

#### InspectorServiceAttributes
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| assessmentRunArn | String   | &check;      |
| rulesPackageArn  | String   | &check;      |
| schemaVersion    | Int      | &check;      |

#### NetworkInterface
| **Name**           | **Type**            | **Nullable** |
| ------------------ | ------------------- | ------------ |
| ipv6Addresses      | List<String>        | &check;      |
| networkInterfaceId | String              | &check;      |
| privateDnsName     | String              | &check;      |
| privateIpAddress   | String              | &check;      |
| privateIpAddresses | List<PrivateIp>     | &check;      |
| publicDnsName      | String              | &check;      |
| publicIp           | String              | &check;      |
| securityGroups     | List<SecurityGroup> | &check;      |
| subnetId           | String              | &check;      |
| vpcId              | String              | &check;      |

#### PrivateIp
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| privateDnsName   | String   | &check;      |
| privateIpAddress | String   | &check;      |

#### SecurityGroup
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| groupId   | String   | &check;      |
| groupName | String   | &check;      |
