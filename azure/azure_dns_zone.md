---
description: Azure Dns Zone
---
azure_dns_zone
--------------

| **Name**                       | **Type**                  | **Nullable** |
| ------------------------------ | ------------------------- | ------------ |
| accessType                     | String                    | &check;      |
| eTag                           | String                    | &check;      |
| id                             | String                    | &cross;      |
| location                       | String                    | &cross;      |
| maxNumberOfRecordSets          | Long                      | &check;      |
| maxNumberOfRecordsPerRecordSet | Long                      | &check;      |
| name                           | String                    | &cross;      |
| nameServers                    | List<String>              | &check;      |
| numberOfRecordSets             | Long                      | &check;      |
| recordSets                     | List<DnsRecordSet>        | &check;      |
| registrationVirtualNetworks    | List<PrivateDnsZoneGroup> | &check;      |
| resolutionVirtualNetworks      | List<PrivateDnsZoneGroup> | &check;      |
| resourceGroupName              | String                    | &cross;      |
| subscriptionId                 | String                    | &cross;      |
| tags                           | Map<String,String>        | &cross;      |
| type                           | String                    | &cross;      |

#### CaaRecord
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| flags    | Int      | &check;      |
| tag      | String   | &check;      |
| value    | String   | &check;      |

#### DnsRecordSet
| **Name**          | **Type**           | **Nullable** |
| ----------------- | ------------------ | ------------ |
| caaRecords        | List<CaaRecord>    | &check;      |
| canonicalName     | String             | &check;      |
| etag              | String             | &check;      |
| fqdn              | String             | &check;      |
| ipv4Address       | List<String>       | &check;      |
| ipv6Address       | List<String>       | &check;      |
| metadata          | Map<String,String> | &check;      |
| mxRecords         | List<MxRecord>     | &check;      |
| nameServers       | List<String>       | &check;      |
| provisioningState | String             | &check;      |
| recordType        | String             | &check;      |
| soaRecord         | SoaRecord          | &check;      |
| srvRecords        | List<SrvRecord>    | &check;      |
| targetDomainNames | List<String>       | &check;      |
| ttl               | Long               | &cross;      |
| txtRecords        | List<TxtRecord>    | &check;      |

#### MxRecord
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| exchange   | String   | &check;      |
| preference | Int      | &check;      |

#### PrivateDnsZoneConfig
| **Name**         | **Type**        | **Nullable** |
| ---------------- | --------------- | ------------ |
| name             | String          | &cross;      |
| privateDnsZoneId | String          | &check;      |
| recordSets       | List<RecordSet> | &check;      |

#### PrivateDnsZoneGroup
| **Name**              | **Type**                   | **Nullable** |
| --------------------- | -------------------------- | ------------ |
| eTag                  | String                     | &check;      |
| id                    | String                     | &cross;      |
| name                  | String                     | &cross;      |
| privateDnsZoneConfigs | List<PrivateDnsZoneConfig> | &check;      |
| provisioningState     | String                     | &check;      |

#### RecordSet
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| fqdn              | String       | &check;      |
| ipAddresses       | List<String> | &check;      |
| provisioningState | String       | &check;      |
| recordSetName     | String       | &check;      |
| recordType        | String       | &check;      |
| ttl               | Int          | &check;      |

#### SoaRecord
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| email        | String   | &check;      |
| expireTime   | Long     | &check;      |
| host         | String   | &check;      |
| minimumTtl   | Long     | &check;      |
| refreshTime  | Long     | &check;      |
| retryTime    | Long     | &check;      |
| serialNumber | Long     | &check;      |

#### SrvRecord
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| port     | Int      | &check;      |
| priority | Int      | &check;      |
| target   | String   | &check;      |
| weight   | Int      | &check;      |

#### TxtRecord
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| value    | List<String> | &check;      |
