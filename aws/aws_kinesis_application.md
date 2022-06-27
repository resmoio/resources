---
description: Amazon Web Services Kinesis Application
---
aws_kinesis_application
-----------------------

| **Name**                                       | **Type**                                       | **Nullable** |
| ---------------------------------------------- | ---------------------------------------------- | ------------ |
| accountId                                      | String                                         | &cross;      |
| applicationARN                                 | String                                         | &cross;      |
| applicationConfigurationDescription            | JSON                                           | &check;      |
| applicationDescription                         | String                                         | &check;      |
| applicationMaintenanceConfigurationDescription | ApplicationMaintenanceConfigurationDescription | &check;      |
| applicationMode                                | String                                         | &check;      |
| applicationName                                | String                                         | &check;      |
| applicationStatus                              | String                                         | &check;      |
| applicationVersionId                           | Long                                           | &check;      |
| applicationVersionRolledBackFrom               | Long                                           | &check;      |
| applicationVersionRolledBackTo                 | Long                                           | &check;      |
| applicationVersionUpdatedFrom                  | Long                                           | &check;      |
| cloudWatchLoggingOptionDescriptions            | List<CloudWatchLoggingOptionDescription>       | &check;      |
| conditionalToken                               | String                                         | &check;      |
| createTimestamp                                | String                                         | &check;      |
| lastUpdateTimestamp                            | String                                         | &check;      |
| region                                         | String                                         | &cross;      |
| runtimeEnvironment                             | String                                         | &check;      |
| serviceExecutionRole                           | String                                         | &check;      |

#### ApplicationMaintenanceConfigurationDescription
| **Name**                              | **Type** | **Nullable** |
| ------------------------------------- | -------- | ------------ |
| applicationMaintenanceWindowEndTime   | String   | &check;      |
| applicationMaintenanceWindowStartTime | String   | &check;      |

#### CloudWatchLoggingOptionDescription
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| cloudWatchLoggingOptionId | String   | &check;      |
| logStreamARN              | String   | &check;      |
| roleARN                   | String   | &check;      |
