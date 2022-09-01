---
description: Entity Host
---
host
----

| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| cpu                    | String       | &check;      |
| data                   | JSON         | &check;      |
| hostName               | String       | &check;      |
| id                     | String       | &cross;      |
| macAddress             | String       | &check;      |
| memory                 | String       | &check;      |
| operatingSystem        | String       | &check;      |
| operatingSystemVersion | String       | &check;      |
| platform               | String       | &check;      |
| privateDnsName         | String       | &check;      |
| privateIpAddresses     | List<String> | &check;      |
| publicDnsName          | String       | &check;      |
| publicIpAddresses      | List<String> | &check;      |
| referencedType         | String       | &cross;      |
| state                  | State        | &check;      |
| type                   | Type         | &check;      |

#### BasicResource
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| data           | JSON     | &check;      |
| referencedType | String   | &cross;      |

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
