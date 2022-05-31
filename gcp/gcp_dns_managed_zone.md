---
description: Google Cloud Platform DNS Managed Zone
---
gcp_dns_managed_zone
--------------------

| **Name**           | **Type**                      | **Nullable** |
| ------------------ | ----------------------------- | ------------ |
| cloudLoggingConfig | ManagedZoneCloudLoggingConfig | &check;      |
| creationTime       | String                        | &check;      |
| description        | String                        | &check;      |
| dnsName            | String                        | &check;      |
| dnssecConfig       | ManagedZoneDnsSecConfig       | &check;      |
| id                 | String                        | &cross;      |
| kind               | String                        | &check;      |
| labels             | Map<String,String>            | &check;      |
| name               | String                        | &cross;      |
| nameServerSet      | String                        | &check;      |
| nameServers        | List<String>                  | &check;      |
| project            | String                        | &cross;      |
| visibility         | String                        | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### ManagedZoneCloudLoggingConfig
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| enableLogging | Boolean  | &check;      |
| kind          | String   | &check;      |

#### ManagedZoneDnsSecConfig
| **Name**        | **Type**                                 | **Nullable** |
| --------------- | ---------------------------------------- | ------------ |
| defaultKeySpecs | List<ManagedZoneDnsSecConfig.DnsKeySpec> | &check;      |
| kind            | String                                   | &check;      |
| nonExistence    | String                                   | &check;      |
| state           | String                                   | &check;      |

#### ManagedZoneDnsSecConfig.DnsKeySpec
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| algorithm | String   | &check;      |
| keyLength | Long     | &check;      |
| keyType   | String   | &check;      |
| kind      | String   | &check;      |
