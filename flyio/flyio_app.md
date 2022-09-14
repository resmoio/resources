---
description: Flyio App
---
flyio_app
---------

| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| appUrl          | String             | &check;      |
| backupRegions   | List<BackupRegion> | &cross;      |
| createdAt       | String             | &check;      |
| deployed        | Boolean            | &check;      |
| healthChecks    | List<Healthcheck>  | &cross;      |
| hostname        | String             | &check;      |
| id              | String             | &cross;      |
| ipAddresses     | List<IpAddress>    | &cross;      |
| key             | String             | &check;      |
| name            | String             | &check;      |
| organization    | Organization       | &check;      |
| platformVersion | String             | &check;      |
| regions         | List<Region>       | &cross;      |
| runtime         | String             | &check;      |
| services        | List<Service>      | &check;      |
| state           | String             | &check;      |
| status          | String             | &check;      |
| version         | Int                | &check;      |
| vmSize          | VmSize             | &check;      |

#### BackupRegion
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| name     | String   | &check;      |

#### Healthcheck
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| status   | String   | &check;      |
| type     | String   | &check;      |

#### IpAddress
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| address   | String   | &check;      |
| createdAt | String   | &check;      |
| id        | String   | &check;      |
| region    | String   | &check;      |
| type      | String   | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| slug     | String   | &check;      |

#### Region
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| name     | String   | &check;      |

#### Service
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| description     | String             | &check;      |
| hardConcurrency | Int                | &check;      |
| internalPort    | Int                | &check;      |
| ports           | List<Service.Port> | &check;      |
| protocol        | String             | &check;      |
| softConcurrency | Int                | &check;      |

#### Service.Port
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| handlers | List<String> | &check;      |
| port     | Int          | &check;      |

#### VmSize
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| cpuCores    | Int      | &check;      |
| maxMemoryMb | Int      | &check;      |
| memoryGb    | Double   | &check;      |
| name        | String   | &check;      |
| priceMonth  | Double   | &check;      |
