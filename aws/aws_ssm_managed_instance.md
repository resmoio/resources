---
description: Amazon Web Services SSM Managed Instance
---
aws_ssm_managed_instance
------------------------

| **Name**                               | **Type**                              | **Nullable** |
| -------------------------------------- | ------------------------------------- | ------------ |
| accountId                              | String                                | &cross;      |
| activationId                           | String                                | &check;      |
| agentVersion                           | String                                | &check;      |
| associationOverview                    | InstanceAggregatedAssociationOverview | &check;      |
| associationStatus                      | String                                | &check;      |
| computerName                           | String                                | &check;      |
| iamRole                                | String                                | &check;      |
| instanceId                             | String                                | &cross;      |
| ipAddress                              | String                                | &check;      |
| isLatestVersion                        | Boolean                               | &check;      |
| lastAssociationExecutionDate           | String                                | &check;      |
| lastSuccessfulAssociationExecutionDate | String                                | &check;      |
| name                                   | String                                | &check;      |
| pingStatus                             | String                                | &check;      |
| platformName                           | String                                | &check;      |
| platformType                           | String                                | &check;      |
| platformVersion                        | String                                | &check;      |
| region                                 | String                                | &cross;      |
| registrationDate                       | String                                | &check;      |
| resourceType                           | String                                | &check;      |
| sourceId                               | String                                | &check;      |
| sourceType                             | String                                | &check;      |

#### InstanceAggregatedAssociationOverview
| **Name**                                 | **Type**        | **Nullable** |
| ---------------------------------------- | --------------- | ------------ |
| detailedStatus                           | String          | &check;      |
| instanceAssociationStatusAggregatedCount | Map<String,Int> | &check;      |
