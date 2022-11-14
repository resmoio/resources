---
description: Amazon Web Services EMR Instance Fleet
---
aws_emr_instance_fleet
----------------------

| **Name**                    | **Type**                                | **Nullable** |
| --------------------------- | --------------------------------------- | ------------ |
| accountId                   | String                                  | &cross;      |
| accountName                 | String                                  | &check;      |
| id                          | String                                  | &cross;      |
| instanceFleetType           | String                                  | &check;      |
| instanceTypeSpecifications  | List<InstanceTypeSpecification>         | &check;      |
| launchSpecifications        | InstanceFleetProvisioningSpecifications | &check;      |
| name                        | String                                  | &check;      |
| provisionedOnDemandCapacity | Int                                     | &check;      |
| provisionedSpotCapacity     | Int                                     | &check;      |
| region                      | String                                  | &cross;      |
| status                      | InstanceFleetStatus                     | &check;      |
| targetOnDemandCapacity      | Int                                     | &check;      |
| targetSpotCapacity          | Int                                     | &check;      |

#### Configuration
| **Name**       | **Type**           | **Nullable** |
| -------------- | ------------------ | ------------ |
| classification | String             | &check;      |
| properties     | Map<String,String> | &check;      |

#### EbsBlockDevice
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| device              | String              | &check;      |
| volumeSpecification | VolumeSpecification | &check;      |

#### InstanceFleetProvisioningSpecifications
| **Name**              | **Type**                          | **Nullable** |
| --------------------- | --------------------------------- | ------------ |
| onDemandSpecification | OnDemandProvisioningSpecification | &check;      |
| spotSpecification     | SpotProvisioningSpecification     | &check;      |

#### InstanceFleetStateChangeReason
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| message  | String   | &check;      |

#### InstanceFleetStatus
| **Name**          | **Type**                       | **Nullable** |
| ----------------- | ------------------------------ | ------------ |
| state             | String                         | &check;      |
| stateChangeReason | InstanceFleetStateChangeReason | &check;      |
| timeline          | InstanceFleetTimeline          | &check;      |

#### InstanceFleetTimeline
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| creationDateTime | String   | &check;      |
| endDateTime      | String   | &check;      |
| readyDateTime    | String   | &check;      |

#### InstanceTypeSpecification
| **Name**                            | **Type**             | **Nullable** |
| ----------------------------------- | -------------------- | ------------ |
| bidPrice                            | String               | &check;      |
| bidPriceAsPercentageOfOnDemandPrice | Double               | &check;      |
| configurations                      | List<Configuration>  | &check;      |
| customAmiId                         | String               | &check;      |
| ebsBlockDevices                     | List<EbsBlockDevice> | &check;      |
| ebsOptimized                        | Boolean              | &check;      |
| instanceType                        | String               | &check;      |
| weightedCapacity                    | Int                  | &check;      |

#### OnDemandCapacityReservationOptions
| **Name**                            | **Type** | **Nullable** |
| ----------------------------------- | -------- | ------------ |
| capacityReservationPreference       | String   | &check;      |
| capacityReservationResourceGroupArn | String   | &check;      |
| usageStrategy                       | String   | &check;      |

#### OnDemandProvisioningSpecification
| **Name**                   | **Type**                           | **Nullable** |
| -------------------------- | ---------------------------------- | ------------ |
| allocationStrategy         | String                             | &check;      |
| capacityReservationOptions | OnDemandCapacityReservationOptions | &check;      |

#### SpotProvisioningSpecification
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| allocationStrategy     | String   | &check;      |
| blockDurationMinutes   | Int      | &check;      |
| timeoutAction          | String   | &check;      |
| timeoutDurationMinutes | Int      | &check;      |

#### VolumeSpecification
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| iops       | Int      | &check;      |
| sizeInGB   | Int      | &check;      |
| throughput | Int      | &check;      |
| volumeType | String   | &check;      |
