---
description: Amazon Web Services EC2 Instance
---
aws_ec2_instance
----------------

| **Name**                         | **Type**                         | **Nullable** |
| -------------------------------- | -------------------------------- | ------------ |
| accountId                        | String                           | &cross;      |
| amiLaunchIndex                   | Int                              | &cross;      |
| architecture                     | String                           | &check;      |
| blockDeviceMappings              | List<BlockDeviceMapping>         | &cross;      |
| capacityReservationSpecification | CapacityReservationSpecification | &cross;      |
| clientToken                      | String                           | &check;      |
| cpuOptions                       | CpuOptions                       | &cross;      |
| disableApiTermination            | Boolean                          | &check;      |
| ebsOptimized                     | Boolean                          | &cross;      |
| enaSupport                       | Boolean                          | &check;      |
| enclaveOptions                   | EnclaveOptions                   | &cross;      |
| hibernateOptions                 | HibernateOptions                 | &cross;      |
| hypervisor                       | String                           | &check;      |
| iamInstanceProfile               | IamInstanceProfile               | &check;      |
| id                               | String                           | &cross;      |
| imageId                          | String                           | &cross;      |
| keyName                          | String                           | &check;      |
| launchTime                       | String                           | &check;      |
| metadataOptions                  | MetadataOptions                  | &cross;      |
| monitoring                       | Monitoring                       | &cross;      |
| networkInterfaces                | List<NetworkInterface>           | &cross;      |
| placement                        | Placement                        | &cross;      |
| platformDetails                  | String                           | &check;      |
| privateDnsName                   | String                           | &check;      |
| privateDnsNameOptions            | PrivateDnsNameOptions            | &check;      |
| publicIpAddress                  | String                           | &check;      |
| region                           | String                           | &cross;      |
| reservationId                    | String                           | &cross;      |
| rootDeviceName                   | String                           | &check;      |
| rootDeviceType                   | String                           | &check;      |
| securityGroups                   | List<SecurityGroup>              | &cross;      |
| sourceDestCheck                  | Boolean                          | &check;      |
| state                            | State                            | &cross;      |
| stateTransitionReason            | String                           | &check;      |
| subnetId                         | String                           | &check;      |
| tags                             | Map<String,String>               | &cross;      |
| type                             | String                           | &cross;      |
| usageOperation                   | String                           | &check;      |
| usageOperationUpdateTime         | String                           | &check;      |
| virtualizationType               | String                           | &check;      |
| vpcId                            | String                           | &check;      |

#### BlockDeviceMapping
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| attachTime          | String   | &cross;      |
| deleteOnTermination | Boolean  | &cross;      |
| deviceName          | String   | &cross;      |
| status              | String   | &cross;      |
| volumeID            | String   | &cross;      |

#### CapacityReservationSpecification
| **Name**                      | **Type**                                | **Nullable** |
| ----------------------------- | --------------------------------------- | ------------ |
| capacityReservationPreference | String                                  | &check;      |
| target                        | CapacityReservationSpecification.Target | &check;      |

#### CapacityReservationSpecification.Target
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| reservationId    | String   | &cross;      |
| resourceGroupArn | String   | &cross;      |

#### CpuOptions
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| coreCount      | Int      | &check;      |
| threadsPerCode | Int      | &check;      |

#### EnclaveOptions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &cross;      |

#### HibernateOptions
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| configured | Boolean  | &cross;      |

#### IamInstanceProfile
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &cross;      |
| id       | String   | &cross;      |

#### MetadataOptions
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| httpEndpoint            | String   | &check;      |
| httpProtocolIpV6        | String   | &check;      |
| httpPutResponseHopLimit | Int      | &check;      |
| httpTokens              | String   | &check;      |
| state                   | String   | &check;      |

#### Monitoring
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| state    | String   | &cross;      |

#### NetworkInterface
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| id             | String       | &cross;      |
| privateDNS     | String       | &check;      |
| privateIP      | String       | &check;      |
| securityGroups | List<String> | &cross;      |
| subnetID       | String       | &check;      |
| vpcID          | String       | &check;      |

#### Placement
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| availabilityZone | String   | &check;      |
| groupName        | String   | &check;      |
| tenancy          | String   | &check;      |

#### PrivateDnsNameOptions
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| enableResourceNameDnsAAAARecord | Boolean  | &check;      |
| enableResourceNameDnsARecord    | Boolean  | &check;      |
| hostnameType                    | String   | &check;      |

#### SecurityGroup
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| name     | String   | &cross;      |

#### State
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | Int      | &check;      |
| name     | String   | &check;      |
