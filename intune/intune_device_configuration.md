---
description: Intune Device Configuration
---
intune_device_configuration
---------------------------

| **Name**                    | **Type**                              | **Nullable** |
| --------------------------- | ------------------------------------- | ------------ |
| createdDateTime             | String                                | &check;      |
| description                 | String                                | &check;      |
| deviceSettingStateSummaries | List<SettingStateDeviceSummary>       | &check;      |
| deviceStatusOverview        | DeviceConfigurationDeviceOverview     | &check;      |
| deviceStatuses              | List<DeviceConfigurationDeviceStatus> | &check;      |
| displayName                 | String                                | &check;      |
| id                          | String                                | &cross;      |
| lastModifiedDateTime        | String                                | &check;      |
| userStatusOverview          | DeviceConfigurationUserOverview       | &check;      |
| userStatuses                | List<DeviceConfigurationUserStatus>   | &check;      |
| version                     | Int                                   | &check;      |

#### DeviceConfigurationDeviceOverview
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| configurationVersion | Int      | &check;      |
| errorCount           | Int      | &check;      |
| failedCount          | Int      | &check;      |
| lastUpdateDateTime   | String   | &check;      |
| notApplicableCount   | Int      | &check;      |
| pendingCount         | Int      | &check;      |
| successCount         | Int      | &check;      |

#### DeviceConfigurationDeviceStatus
| **Name**                                | **Type** | **Nullable** |
| --------------------------------------- | -------- | ------------ |
| complianceGracePeriodExpirationDateTime | String   | &check;      |
| deviceDisplayName                       | String   | &check;      |
| deviceModel                             | String   | &check;      |
| id                                      | String   | &cross;      |
| lastReportedDateTime                    | String   | &check;      |
| status                                  | String   | &check;      |
| userName                                | String   | &check;      |
| userPrincipalName                       | String   | &check;      |

#### DeviceConfigurationUserOverview
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| configurationVersion | Int      | &check;      |
| errorCount           | Int      | &check;      |
| failedCount          | Int      | &check;      |
| id                   | String   | &cross;      |
| lastUpdateDateTime   | String   | &check;      |
| notApplicableCount   | Int      | &check;      |
| pendingCount         | Int      | &check;      |
| successCount         | Int      | &check;      |

#### DeviceConfigurationUserStatus
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| devicesCount         | Int      | &check;      |
| id                   | String   | &cross;      |
| lastReportedDateTime | String   | &check;      |
| status               | String   | &check;      |
| userDisplayName      | String   | &check;      |
| userPrincipalName    | String   | &check;      |

#### SettingStateDeviceSummary
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| compliantDeviceCount     | Int      | &check;      |
| conflictDeviceCount      | Int      | &check;      |
| errorDeviceCount         | Int      | &check;      |
| id                       | String   | &cross;      |
| instancePath             | String   | &check;      |
| nonCompliantDeviceCount  | Int      | &check;      |
| notApplicableDeviceCount | Int      | &check;      |
| remediatedDeviceCount    | Int      | &check;      |
| settingName              | String   | &check;      |
| unknownDeviceCount       | Int      | &check;      |
