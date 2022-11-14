---
description: Amazon Web Services DMS Replication Instance
---
aws_dms_replication_instance
----------------------------

| **Name**                              | **Type**                         | **Nullable** |
| ------------------------------------- | -------------------------------- | ------------ |
| accountId                             | String                           | &cross;      |
| accountName                           | String                           | &check;      |
| allocatedStorage                      | Int                              | &check;      |
| autoMinorVersionUpgrade               | Boolean                          | &check;      |
| availabilityZone                      | String                           | &check;      |
| dnsNameServers                        | String                           | &check;      |
| engineVersion                         | String                           | &check;      |
| freeUntil                             | String                           | &check;      |
| instanceCreateTime                    | String                           | &check;      |
| kmsKeyId                              | String                           | &check;      |
| multiAZ                               | Boolean                          | &check;      |
| pendingModifiedValues                 | ReplicationPendingModifiedValues | &check;      |
| preferredMaintenanceWindow            | String                           | &check;      |
| publiclyAccessible                    | Boolean                          | &check;      |
| region                                | String                           | &cross;      |
| replicationInstanceArn                | String                           | &cross;      |
| replicationInstanceClass              | String                           | &check;      |
| replicationInstanceIdentifier         | String                           | &check;      |
| replicationInstancePrivateIpAddress   | String                           | &check;      |
| replicationInstancePrivateIpAddresses | List<String>                     | &check;      |
| replicationInstancePublicIpAddress    | String                           | &check;      |
| replicationInstancePublicIpAddresses  | List<String>                     | &check;      |
| replicationInstanceStatus             | String                           | &check;      |
| replicationSubnetGroup                | ReplicationSubnetGroup           | &check;      |
| secondaryAvailabilityZone             | String                           | &check;      |
| vpcSecurityGroups                     | List<VpcSecurityGroupMembership> | &check;      |

#### ReplicationPendingModifiedValues
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| allocatedStorage         | Int      | &check;      |
| engineVersion            | String   | &check;      |
| multiAZ                  | Boolean  | &check;      |
| replicationInstanceClass | String   | &check;      |

#### ReplicationSubnetGroup
| **Name**                          | **Type**     | **Nullable** |
| --------------------------------- | ------------ | ------------ |
| replicationSubnetGroupDescription | String       | &check;      |
| replicationSubnetGroupIdentifier  | String       | &check;      |
| subnetGroupStatus                 | String       | &check;      |
| subnets                           | List<Subnet> | &check;      |
| vpcId                             | String       | &check;      |

#### Subnet
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| subnetAvailabilityZone | String   | &check;      |
| subnetIdentifier       | String   | &check;      |
| subnetStatus           | String   | &check;      |

#### VpcSecurityGroupMembership
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| status             | String   | &check;      |
| vpcSecurityGroupId | String   | &check;      |
