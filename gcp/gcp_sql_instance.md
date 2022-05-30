---
description: Google Cloud Platform SQL Instance
---
gcp_sql_instance
----------------

| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| backendType                 | String                      | &check;      |
| connectionName              | String                      | &check;      |
| createTime                  | String                      | &check;      |
| currentDiskSize             | Long                        | &check;      |
| databaseInstalledVersion    | String                      | &check;      |
| databaseVersion             | String                      | &check;      |
| diskEncryptionConfiguration | DiskEncryptionConfiguration | &check;      |
| diskEncryptionStatus        | DiskEncryptionStatus        | &check;      |
| failoverReplica             | FailoverReplica             | &check;      |
| gceZone                     | String                      | &check;      |
| instanceType                | String                      | &check;      |
| ipAddresses                 | List<IpMapping>             | &check;      |
| ipv6Address                 | String                      | &check;      |
| kind                        | String                      | &check;      |
| masterInstanceName          | String                      | &check;      |
| maxDiskSize                 | Long                        | &check;      |
| name                        | String                      | &cross;      |
| onPremisesConfiguration     | OnPremisesConfiguration     | &check;      |
| outOfDiskReport             | SqlOutOfDiskReport          | &check;      |
| project                     | String                      | &cross;      |
| region                      | String                      | &check;      |
| replicaConfiguration        | ReplicaConfiguration        | &check;      |
| replicaNames                | List<String>                | &check;      |
| scheduledMaintenance        | SqlScheduledMaintenance     | &check;      |
| secondaryGceZone            | String                      | &check;      |
| serverCaCert                | SslCert                     | &check;      |
| settings                    | JSON                        | &check;      |
| state                       | String                      | &check;      |
| suspensionReason            | List<String>                | &check;      |

#### DiskEncryptionConfiguration
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| kind       | String   | &check;      |
| kmsKeyName | String   | &check;      |

#### DiskEncryptionStatus
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| kind              | String   | &check;      |
| kmsKeyVersionName | String   | &check;      |

#### FailoverReplica
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| available | Boolean  | &check;      |
| name      | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### IpMapping
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| ipAddress    | String   | &check;      |
| timeToRetire | String   | &check;      |
| type         | String   | &check;      |

#### OnPremisesConfiguration
| **Name**          | **Type**                                  | **Nullable** |
| ----------------- | ----------------------------------------- | ------------ |
| caCertificate     | String                                    | &check;      |
| clientCertificate | String                                    | &check;      |
| clientKey         | String                                    | &check;      |
| dumpFilePath      | String                                    | &check;      |
| hostPort          | String                                    | &check;      |
| kind              | String                                    | &check;      |
| sourceInstance    | OnPremisesConfiguration.InstanceReference | &check;      |
| username          | String                                    | &check;      |

#### OnPremisesConfiguration.InstanceReference
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| project  | String   | &check;      |
| region   | String   | &check;      |

#### ReplicaConfiguration
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| failoverTarget | Boolean  | &check;      |
| kind           | String   | &check;      |

#### SqlOutOfDiskReport
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| sqlMinRecommendedIncreaseSizeGb | Int      | &check;      |
| sqlOutOfDiskState               | String   | &check;      |

#### SqlScheduledMaintenance
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| canDefer             | Boolean  | &check;      |
| canReschedule        | Boolean  | &check;      |
| scheduleDeadlineTime | String   | &check;      |
| startTime            | String   | &check;      |

#### SslCert
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| certSerialNumber | String   | &check;      |
| commonName       | String   | &check;      |
| createTime       | String   | &check;      |
| expirationTime   | String   | &check;      |
| instance         | String   | &check;      |
| kind             | String   | &check;      |
