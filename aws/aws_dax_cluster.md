---
description: Amazon Web Services DAX Cluster
---
aws_dax_cluster
---------------

| **Name**                      | **Type**                      | **Nullable** |
| ----------------------------- | ----------------------------- | ------------ |
| accountId                     | String                        | &cross;      |
| accountName                   | String                        | &check;      |
| activeNodes                   | Int                           | &check;      |
| clusterArn                    | String                        | &cross;      |
| clusterDiscoveryEndpoint      | Endpoint                      | &check;      |
| clusterEndpointEncryptionType | String                        | &check;      |
| clusterName                   | String                        | &check;      |
| description                   | String                        | &check;      |
| iamRoleArn                    | String                        | &check;      |
| nodeIdsToRemove               | List<String>                  | &check;      |
| nodeType                      | String                        | &check;      |
| nodes                         | List<Node>                    | &check;      |
| notificationConfiguration     | NotificationConfiguration     | &check;      |
| parameterGroup                | ParameterGroupStatus          | &check;      |
| preferredMaintenanceWindow    | String                        | &check;      |
| region                        | String                        | &cross;      |
| securityGroups                | List<SecurityGroupMembership> | &check;      |
| sseDescription                | SSEDescription                | &check;      |
| status                        | String                        | &check;      |
| subnetGroup                   | String                        | &check;      |
| totalNodes                    | Int                           | &check;      |

#### Endpoint
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| address  | String   | &check;      |
| port     | Int      | &check;      |
| url      | String   | &check;      |

#### Node
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| availabilityZone     | String   | &check;      |
| endpoint             | Endpoint | &check;      |
| nodeCreateTime       | String   | &check;      |
| nodeId               | String   | &check;      |
| nodeStatus           | String   | &check;      |
| parameterGroupStatus | String   | &check;      |

#### NotificationConfiguration
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| topicArn    | String   | &check;      |
| topicStatus | String   | &check;      |

#### ParameterGroupStatus
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| nodeIdsToReboot      | List<String> | &check;      |
| parameterApplyStatus | String       | &check;      |
| parameterGroupName   | String       | &check;      |

#### SSEDescription
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| status   | String   | &check;      |

#### SecurityGroupMembership
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| securityGroupIdentifier | String   | &check;      |
| status                  | String   | &check;      |
