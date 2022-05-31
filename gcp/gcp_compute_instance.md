---
description: Google Cloud Platform Compute Instance
---
gcp_compute_instance
--------------------

| **Name**                        | **Type**                        | **Nullable** |
| ------------------------------- | ------------------------------- | ------------ |
| advancedMachineFeatures         | AdvancedMachineFeatures         | &check;      |
| canIpForward                    | Boolean                         | &check;      |
| confidentialInstanceConfig      | ConfidentialInstanceConfig      | &check;      |
| cpuPlatform                     | String                          | &check;      |
| creationTimestamp               | String                          | &check;      |
| deletionProtection              | Boolean                         | &check;      |
| description                     | String                          | &check;      |
| disks                           | List<AttachedDisk>              | &check;      |
| displayDevice                   | DisplayDevice                   | &check;      |
| guestAccelerators               | List<AcceleratorConfig>         | &check;      |
| hostname                        | String                          | &check;      |
| id                              | Long                            | &cross;      |
| kind                            | String                          | &check;      |
| labels                          | Map<String,String>              | &check;      |
| lastStartTimestamp              | String                          | &check;      |
| lastStopTimestamp               | String                          | &check;      |
| lastSuspendedTimestamp          | String                          | &check;      |
| machineType                     | String                          | &check;      |
| metadata                        | JSON                            | &check;      |
| minCpuPlatform                  | String                          | &check;      |
| name                            | String                          | &cross;      |
| networkInterfaces               | List<NetworkInterface>          | &check;      |
| privateIpv6GoogleAccess         | String                          | &check;      |
| project                         | String                          | &cross;      |
| reservationAffinity             | ReservationAffinity             | &check;      |
| resourcePolicies                | List<String>                    | &check;      |
| satisfiesPzs                    | Boolean                         | &check;      |
| scheduling                      | Scheduling                      | &check;      |
| serviceAccounts                 | List<ServiceAccount>            | &check;      |
| shieldedInstanceConfig          | ShieldedInstanceConfig          | &check;      |
| shieldedInstanceIntegrityPolicy | ShieldedInstanceIntegrityPolicy | &check;      |
| startRestricted                 | Boolean                         | &check;      |
| status                          | String                          | &check;      |
| statusMessage                   | String                          | &check;      |
| tags                            | JSON                            | &check;      |
| zone                            | String                          | &cross;      |

#### AcceleratorConfig
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| acceleratorCount | Int      | &check;      |
| acceleratorType  | String   | &cross;      |

#### AccessConfig
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| externalIpv6             | String   | &check;      |
| externalIpv6PrefixLength | Int      | &check;      |
| kind                     | String   | &check;      |
| name                     | String   | &check;      |
| natIP                    | String   | &check;      |
| networkTier              | String   | &check;      |
| publicPtrDomainName      | String   | &check;      |
| setPublicPtr             | Boolean  | &check;      |
| type                     | String   | &check;      |

#### AdvancedMachineFeatures
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| enableNestedVirtualization | Boolean  | &check;      |
| threadsPerCore             | Int      | &check;      |

#### AliasIpRange
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| ipCidrRange         | String   | &check;      |
| subnetworkRangeName | String   | &check;      |

#### AttachedDisk
| **Name**          | **Type**              | **Nullable** |
| ----------------- | --------------------- | ------------ |
| autoDelete        | Boolean               | &check;      |
| boot              | Boolean               | &check;      |
| deviceName        | String                | &check;      |
| diskEncryptionKey | CustomerEncryptionKey | &check;      |
| diskSizeGb        | Long                  | &check;      |
| guestOsFeatures   | List<GuestOsFeature>  | &check;      |
| index             | Int                   | &check;      |
| interface_        | String                | &check;      |
| kind              | String                | &check;      |
| licenses          | List<String>          | &check;      |
| mode              | String                | &check;      |
| source            | String                | &check;      |
| type              | String                | &check;      |

#### ConfidentialInstanceConfig
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| enableConfidentialCompute | Boolean  | &check;      |

#### CustomerEncryptionKey
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| kmsKeyName           | String   | &check;      |
| kmsKeyServiceAccount | String   | &check;      |

#### DisplayDevice
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| enableDisplay | Boolean  | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### GuestOsFeature
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &cross;      |

#### NetworkInterface
| **Name**          | **Type**           | **Nullable** |
| ----------------- | ------------------ | ------------ |
| accessConfigs     | List<AccessConfig> | &check;      |
| aliasIpRanges     | List<AliasIpRange> | &check;      |
| ipv6AccessConfigs | List<AccessConfig> | &check;      |
| ipv6AccessType    | String             | &check;      |
| ipv6Address       | String             | &check;      |
| kind              | String             | &check;      |
| name              | String             | &check;      |
| network           | String             | &check;      |
| networkIP         | String             | &check;      |
| nicType           | String             | &check;      |
| queueCount        | Int                | &check;      |
| stackType         | String             | &check;      |
| subnetwork        | String             | &check;      |

#### ReservationAffinity
| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| consumeReservationType | String       | &check;      |
| key                    | String       | &check;      |
| values                 | List<String> | &check;      |

#### Scheduling
| **Name**          | **Type**                     | **Nullable** |
| ----------------- | ---------------------------- | ------------ |
| automaticRestart  | Boolean                      | &check;      |
| locationHint      | String                       | &check;      |
| minNodeCpus       | Int                          | &check;      |
| nodeAffinities    | List<SchedulingNodeAffinity> | &check;      |
| onHostMaintenance | String                       | &check;      |
| preemptible       | Boolean                      | &check;      |

#### SchedulingNodeAffinity
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &check;      |
| operator | String       | &check;      |
| values   | List<String> | &check;      |

#### ServiceAccount
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| email    | String       | &check;      |
| scopes   | List<String> | &check;      |

#### ShieldedInstanceConfig
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| enableIntegrityMonitoring | Boolean  | &check;      |
| enableSecureBoot          | Boolean  | &check;      |
| enableVtpm                | Boolean  | &check;      |

#### ShieldedInstanceIntegrityPolicy
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| updateAutoLearnPolicy | Boolean  | &check;      |
