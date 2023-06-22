---
description: Intune Device Compliance Policy
---
intune_device_compliance_policy
-------------------------------

| **Name**                    | **Type**                                     | **Nullable** |
| --------------------------- | -------------------------------------------- | ------------ |
| createdDateTime             | String                                       | &check;      |
| description                 | String                                       | &check;      |
| deviceSettingStateSummaries | List<SettingStateDeviceSummary>              | &check;      |
| deviceStatusOverview        | DeviceComplianceDeviceOverview               | &check;      |
| deviceStatuses              | List<DeviceComplianceDeviceStatus>           | &check;      |
| displayName                 | String                                       | &check;      |
| id                          | String                                       | &cross;      |
| lastModifiedDateTime        | String                                       | &check;      |
| scheduledActionsForRule     | List<DeviceComplianceScheduledActionForRule> | &check;      |
| userStatusOverview          | DeviceComplianceUserOverview                 | &check;      |
| userStatuses                | List<DeviceComplianceUserStatus>             | &check;      |
| version                     | Int                                          | &check;      |

#### DeviceComplianceActionItem
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| actionType                | String       | &check;      |
| gracePeriodHours          | Int          | &check;      |
| id                        | String       | &cross;      |
| notificationMessageCCList | List<String> | &check;      |
| notificationTemplateId    | String       | &check;      |

#### DeviceComplianceDeviceOverview
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

#### DeviceComplianceDeviceStatus
| **Name**                                | **Type** | **Nullable** |
| --------------------------------------- | -------- | ------------ |
| complianceGracePeriodExpirationDateTime | String   | &check;      |
| deviceDisplayName                       | String   | &check;      |
| deviceModel                             | String   | &check;      |
| lastReportedDateTime                    | String   | &check;      |
| status                                  | String   | &check;      |
| userName                                | String   | &check;      |
| userPrincipalName                       | String   | &check;      |

#### DeviceComplianceScheduledActionForRule
| **Name**                      | **Type**                         | **Nullable** |
| ----------------------------- | -------------------------------- | ------------ |
| id                            | String                           | &cross;      |
| ruleName                      | String                           | &check;      |
| scheduledActionConfigurations | List<DeviceComplianceActionItem> | &check;      |

#### DeviceComplianceUserOverview
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

#### DeviceComplianceUserStatus
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
