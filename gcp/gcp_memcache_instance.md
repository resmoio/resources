---
description: Google Cloud Platform Memcache Instance
---
gcp_memcache_instance
---------------------

| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| authorizedNetwork   | String              | &check;      |
| createTime          | String              | &check;      |
| discoveryEndpoint   | String              | &check;      |
| displayName         | String              | &check;      |
| labels              | Map<String,String>  | &check;      |
| maintenancePolicy   | MaintenancePolicy   | &check;      |
| maintenanceSchedule | MaintenanceSchedule | &check;      |
| memcacheFullVersion | String              | &check;      |
| memcacheNodes       | List<Node>          | &check;      |
| memcacheVersion     | String              | &check;      |
| name                | String              | &cross;      |
| nodeConfig          | NodeConfig          | &check;      |
| nodeCount           | Int                 | &check;      |
| parameters          | MemcacheParameters  | &check;      |
| project             | String              | &cross;      |
| state               | String              | &check;      |
| updateTime          | String              | &check;      |
| zones               | List<String>        | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### MaintenancePolicy
| **Name**                | **Type**                                        | **Nullable** |
| ----------------------- | ----------------------------------------------- | ------------ |
| createTime              | String                                          | &check;      |
| description             | String                                          | &check;      |
| updateTime              | String                                          | &check;      |
| weeklyMaintenanceWindow | List<MaintenancePolicy.WeeklyMaintenanceWindow> | &check;      |

#### MaintenancePolicy.WeeklyMaintenanceWindow
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| day       | String   | &check;      |
| duration  | String   | &check;      |
| startTime | String   | &check;      |

#### MaintenanceSchedule
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| endTime              | String   | &check;      |
| scheduleDeadlineTime | String   | &check;      |
| startTime            | String   | &check;      |

#### MemcacheParameters
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| id       | String             | &check;      |
| params   | Map<String,String> | &check;      |

#### Node
| **Name**   | **Type**           | **Nullable** |
| ---------- | ------------------ | ------------ |
| host       | String             | &check;      |
| nodeId     | String             | &cross;      |
| parameters | MemcacheParameters | &check;      |
| port       | Int                | &check;      |
| state      | String             | &check;      |
| zone       | String             | &check;      |

#### NodeConfig
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| cpuCount     | Int      | &check;      |
| memorySizeMb | Int      | &check;      |
