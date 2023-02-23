---
description: Entity Host
---
host
----

| **Name**               | **Type**           | **Nullable** |
| ---------------------- | ------------------ | ------------ |
| cpu                    | String             | &check;      |
| hostName               | String             | &check;      |
| id                     | String             | &cross;      |
| macAddress             | String             | &check;      |
| memory                 | String             | &check;      |
| operatingSystem        | String             | &check;      |
| operatingSystemVersion | String             | &check;      |
| platform               | String             | &check;      |
| privateDnsName         | String             | &check;      |
| privateIpAddresses     | List<String>       | &check;      |
| publicDnsName          | String             | &check;      |
| publicIpAddresses      | List<String>       | &check;      |
| referencedResource     | ReferencedResource | &check;      |
| referencedType         | String             | &cross;      |
| state                  | String             | &check;      |
| type                   | String             | &check;      |

#### BasicResource
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| referencedResource | ReferencedResource | &check;      |
| referencedType     | String             | &cross;      |

#### ReferencedResource
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| groupKey      | String   | &cross;      |
| integrationId | String   | &cross;      |
| recordId      | String   | &cross;      |
| resourceId    | String   | &cross;      |
| resourceType  | String   | &cross;      |

#### State
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |

#### Type
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| ordinal  | Int      | &cross;      |
