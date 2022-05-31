---
description: Amazon Web Services Autoscaling Launch Configuration
---
aws_autoscaling_launch_configuration
------------------------------------

| **Name**                     | **Type**                 | **Nullable** |
| ---------------------------- | ------------------------ | ------------ |
| accountId                    | String                   | &cross;      |
| arn                          | String                   | &cross;      |
| associatePublicIpAddress     | Boolean                  | &check;      |
| blockDeviceMappings          | List<BlockDeviceMapping> | &check;      |
| classicLinkVPCId             | String                   | &check;      |
| classicLinkVPCSecurityGroups | List<String>             | &check;      |
| createdTime                  | String                   | &check;      |
| ebsOptimized                 | Boolean                  | &check;      |
| iamInstanceProfile           | String                   | &check;      |
| imageId                      | String                   | &check;      |
| instanceMonitoring           | Boolean                  | &check;      |
| instanceType                 | String                   | &check;      |
| kernelId                     | String                   | &check;      |
| keyName                      | String                   | &check;      |
| metadataOptions              | InstanceMetadataOptions  | &check;      |
| name                         | String                   | &cross;      |
| placementTenancy             | String                   | &check;      |
| ramdiskId                    | String                   | &check;      |
| region                       | String                   | &cross;      |
| securityGroups               | List<String>             | &check;      |
| spotPrice                    | String                   | &check;      |
| userData                     | String                   | &check;      |

#### BlockDeviceMapping
| **Name**    | **Type**               | **Nullable** |
| ----------- | ---------------------- | ------------ |
| deviceName  | String                 | &check;      |
| ebs         | BlockDeviceMapping.Ebs | &check;      |
| noDevice    | Boolean                | &check;      |
| virtualName | String                 | &check;      |

#### BlockDeviceMapping.Ebs
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| deleteOnTermination | Boolean  | &check;      |
| encrypted           | Boolean  | &check;      |
| iops                | Int      | &check;      |
| snapshotId          | String   | &check;      |
| throughput          | Int      | &check;      |
| volumeSize          | Int      | &check;      |
| volumeType          | String   | &check;      |

#### InstanceMetadataOptions
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| httpEndpoint            | String   | &check;      |
| httpPutResponseHopLimit | Int      | &check;      |
| httpTokens              | String   | &check;      |
