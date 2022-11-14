---
description: Amazon Web Services EMR Instance
---
aws_emr_instance
----------------

| **Name**         | **Type**        | **Nullable** |
| ---------------- | --------------- | ------------ |
| accountId        | String          | &cross;      |
| accountName      | String          | &check;      |
| clusterId        | String          | &check;      |
| ebsVolumes       | List<EbsVolume> | &check;      |
| ec2InstanceId    | String          | &check;      |
| id               | String          | &cross;      |
| instanceFleetId  | String          | &check;      |
| instanceGroupId  | String          | &check;      |
| instanceType     | String          | &check;      |
| market           | String          | &check;      |
| privateDnsName   | String          | &check;      |
| privateIpAddress | String          | &check;      |
| publicDnsName    | String          | &check;      |
| publicIpAddress  | String          | &check;      |
| region           | String          | &cross;      |
| status           | InstanceStatus  | &check;      |

#### EbsVolume
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| device   | String   | &check;      |
| volumeId | String   | &check;      |

#### InstanceStateChangeReason
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | String   | &check;      |
| message  | String   | &check;      |

#### InstanceStatus
| **Name**          | **Type**                  | **Nullable** |
| ----------------- | ------------------------- | ------------ |
| state             | String                    | &check;      |
| stateChangeReason | InstanceStateChangeReason | &check;      |
| timeline          | InstanceTimeline          | &check;      |

#### InstanceTimeline
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| creationDateTime | String   | &check;      |
| endDateTime      | String   | &check;      |
| readyDateTime    | String   | &check;      |
