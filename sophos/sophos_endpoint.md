---
description: Sophos Endpoint
---
sophos_endpoint
---------------

| **Name**                | **Type**              | **Nullable** |
| ----------------------- | --------------------- | ------------ |
| assignedProducts        | List<AssignedProduct> | &check;      |
| associatedPerson        | AssociatedPerson      | &check;      |
| cloud                   | String                | &check;      |
| encryption              | Encryption            | &check;      |
| group                   | Group                 | &check;      |
| health                  | Health                | &check;      |
| hostname                | String                | &cross;      |
| id                      | String                | &cross;      |
| ipv4Addresses           | List<String>          | &check;      |
| ipv6Addresses           | List<String>          | &check;      |
| isolation               | Isolation             | &check;      |
| lastSeenAt              | String                | &check;      |
| lockdown                | Lockdown              | &check;      |
| macAddresses            | List<String>          | &check;      |
| online                  | String                | &check;      |
| os                      | Os                    | &check;      |
| tamperProtectionEnabled | Boolean               | &check;      |
| tenant                  | Tenant                | &cross;      |
| type                    | String                | &cross;      |

#### AssignedProduct
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &cross;      |
| status   | String   | &check;      |
| version  | String   | &cross;      |

#### AssociatedPerson
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| viaLogin | String   | &check;      |

#### Cloud
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| instanceId | String   | &cross;      |
| provider   | String   | &cross;      |

#### Encryption
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| volumes  | List<Volume> | &cross;      |

#### Group
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |

#### Health
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| overall  | String   | &cross;      |
| services | Services | &cross;      |
| threats  | Threats  | &cross;      |

#### Isolation
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| adminIsolated | Boolean  | &check;      |
| selfIsolated  | Boolean  | &check;      |
| status        | String   | &cross;      |

#### Lockdown
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| status       | String   | &cross;      |
| updateStatus | String   | &check;      |

#### Os
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| build        | Int      | &check;      |
| isServer     | Boolean  | &check;      |
| majorVersion | Int      | &check;      |
| minorVersion | Int      | &check;      |
| name         | String   | &cross;      |
| platform     | String   | &cross;      |

#### ServiceDetails
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| status   | String   | &cross;      |

#### Services
| **Name**       | **Type**             | **Nullable** |
| -------------- | -------------------- | ------------ |
| serviceDetails | List<ServiceDetails> | &cross;      |
| status         | String               | &cross;      |

#### Tenant
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &check;      |

#### Threats
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| status   | String   | &cross;      |

#### Volume
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| status   | String   | &cross;      |
| volumeId | String   | &cross;      |
