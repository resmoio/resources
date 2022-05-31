---
description: Amazon Web Services Autoscaling Group
---
aws_autoscaling_group
---------------------

| **Name**                         | **Type**               | **Nullable** |
| -------------------------------- | ---------------------- | ------------ |
| accountId                        | String                 | &cross;      |
| arn                              | String                 | &cross;      |
| availabilityZones                | List<String>           | &check;      |
| capacityRebalance                | Boolean                | &check;      |
| context                          | String                 | &check;      |
| createdTime                      | String                 | &check;      |
| defaultCooldown                  | Int                    | &check;      |
| desiredCapacity                  | Int                    | &check;      |
| desiredCapacityType              | String                 | &check;      |
| enabledMetrics                   | List<EnabledMetric>    | &check;      |
| healthCheckGracePeriod           | Int                    | &check;      |
| healthCheckType                  | String                 | &check;      |
| launchConfigurationName          | String                 | &check;      |
| launchTemplate                   | LaunchTemplateSpec     | &check;      |
| loadBalancerNames                | List<String>           | &check;      |
| maxInstanceLifetime              | Int                    | &check;      |
| maxSize                          | Int                    | &check;      |
| minSize                          | Int                    | &check;      |
| name                             | String                 | &cross;      |
| newInstancesProtectedFromScaleIn | Boolean                | &check;      |
| placementGroup                   | String                 | &check;      |
| predictedCapacity                | Int                    | &check;      |
| region                           | String                 | &cross;      |
| serviceLinkedRoleARN             | String                 | &check;      |
| status                           | String                 | &check;      |
| suspendedProcesses               | List<SuspendedProcess> | &check;      |
| targetGroupARNs                  | List<String>           | &check;      |
| terminationPolicies              | List<String>           | &check;      |
| vpcZoneIdentifier                | String                 | &check;      |
| warmPoolConfiguration            | WarmPoolConfiguration  | &check;      |
| warmPoolSize                     | Int                    | &check;      |

#### EnabledMetric
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| granularity | String   | &check;      |
| metric      | String   | &check;      |

#### LaunchTemplateSpec
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| launchTemplateId   | String   | &check;      |
| launchTemplateName | String   | &check;      |
| version            | String   | &check;      |

#### SuspendedProcess
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| processName      | String   | &check;      |
| suspensionReason | String   | &check;      |

#### WarmPoolConfiguration
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| maxGroupPreparedCapacity | Int      | &check;      |
| minSize                  | Int      | &check;      |
| poolState                | String   | &check;      |
| status                   | String   | &check;      |
