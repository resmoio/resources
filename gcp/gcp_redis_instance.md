---
description: Google Cloud Platform Redis Instance
---
gcp_redis_instance
------------------

| **Name**               | **Type**             | **Nullable** |
| ---------------------- | -------------------- | ------------ |
| alternativeLocationId  | String               | &check;      |
| authEnabled            | Boolean              | &check;      |
| authorizedNetwork      | String               | &check;      |
| connectMode            | String               | &check;      |
| createTime             | String               | &check;      |
| currentLocationId      | String               | &check;      |
| displayName            | String               | &check;      |
| host                   | String               | &check;      |
| labels                 | Map<String,String>   | &check;      |
| locationId             | String               | &check;      |
| maintenancePolicy      | MaintenancePolicy    | &check;      |
| maintenanceSchedule    | MaintenanceSchedule  | &check;      |
| memorySizeGb           | Int                  | &check;      |
| name                   | String               | &cross;      |
| nodes                  | List<NodeInfo>       | &check;      |
| persistenceConfig      | PersistenceConfig    | &check;      |
| persistenceIamIdentity | String               | &check;      |
| port                   | Int                  | &check;      |
| project                | String               | &cross;      |
| readEndpoint           | String               | &check;      |
| readEndpointPort       | Int                  | &check;      |
| readReplicasMode       | String               | &check;      |
| redisConfigs           | Map<String,String>   | &check;      |
| redisVersion           | String               | &check;      |
| replicaCount           | Int                  | &check;      |
| reservedIpRange        | String               | &check;      |
| secondaryIpRange       | String               | &check;      |
| serverCaCerts          | List<TlsCertificate> | &check;      |
| state                  | String               | &check;      |
| tier                   | String               | &check;      |
| transitEncryptionMode  | String               | &check;      |

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
| canReschedule        | Boolean  | &check;      |
| endTime              | String   | &check;      |
| scheduleDeadlineTime | String   | &check;      |
| startTime            | String   | &check;      |

#### NodeInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| zone     | String   | &check;      |

#### PersistenceConfig
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| persistenceMode      | String   | &check;      |
| rdbNextSnapshotTime  | String   | &check;      |
| rdbSnapshotPeriod    | String   | &check;      |
| rdbSnapshotStartTime | String   | &check;      |

#### TlsCertificate
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| cert         | String   | &check;      |
| createTime   | String   | &check;      |
| expireTime   | String   | &check;      |
| serialNumber | String   | &check;      |
