---
description: Amazon Web Services Autoscaling Group
---
aws_autoscaling_group
---------------------

| **Name**                         | **Type**               | **Nullable** |
| -------------------------------- | ---------------------- | ------------ |
| accountId                        | String                 | &cross;      |
| accountName                      | String                 | &check;      |
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
| mixedInstancesPolicy             | MixedInstancePolicy    | &check;      |
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

#### InstancesDistribution
| **Name**                            | **Type** | **Nullable** |
| ----------------------------------- | -------- | ------------ |
| onDemandAllocationStrategy          | String   | &check;      |
| onDemandBaseCapacity                | Int      | &check;      |
| onDemandPercentageAboveBaseCapacity | Int      | &check;      |
| spotAllocationStrategy              | String   | &check;      |
| spotInstancePools                   | Int      | &check;      |
| spotMaxPrice                        | String   | &check;      |

#### LaunchTemplate
| **Name**                    | **Type**                     | **Nullable** |
| --------------------------- | ---------------------------- | ------------ |
| launchTemplateSpecification | LaunchTemplateSpecification  | &check;      |
| overrides                   | List<LaunchTemplateOverride> | &check;      |

#### LaunchTemplateOverride
| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| instanceRequirements        | JSON                        | &check;      |
| instanceType                | String                      | &check;      |
| launchTemplateSpecification | LaunchTemplateSpecification | &check;      |
| weightedCapacity            | String                      | &check;      |

#### LaunchTemplateSpec
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| launchTemplateId   | String   | &check;      |
| launchTemplateName | String   | &check;      |
| version            | String   | &check;      |

#### LaunchTemplateSpecification
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| launchTemplateId   | String   | &check;      |
| launchTemplateName | String   | &check;      |
| version            | String   | &check;      |

#### MixedInstancePolicy
| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| instancesDistribution | InstancesDistribution | &check;      |
| launchTemplate        | LaunchTemplate        | &check;      |

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
