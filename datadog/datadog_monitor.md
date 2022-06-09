---
description: Datadog Monitor
---
datadog_monitor
---------------

| **Name**        | **Type**               | **Nullable** |
| --------------- | ---------------------- | ------------ |
| createdAt       | String                 | &check;      |
| creator         | Creator                | &check;      |
| deleted         | String                 | &check;      |
| id              | String                 | &cross;      |
| message         | String                 | &check;      |
| multi           | Boolean                | &check;      |
| name            | String                 | &check;      |
| options         | Options                | &check;      |
| overallState    | Value                  | &check;      |
| priority        | Long                   | &check;      |
| query           | String                 | &check;      |
| restrictedRoles | List<String>           | &check;      |
| stateGroups     | Map<String,StateGroup> | &check;      |
| tags            | List<String>           | &check;      |
| type            | Value                  | &check;      |

#### Aggregation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupBy  | String   | &check;      |
| metric   | String   | &check;      |
| type     | String   | &check;      |

#### Creator
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &check;      |
| handle   | String   | &check;      |
| name     | String   | &check;      |

#### Options
| **Name**                       | **Type**         | **Nullable** |
| ------------------------------ | ---------------- | ------------ |
| aggregation                    | Aggregation      | &check;      |
| deviceIds                      | List<Value>      | &check;      |
| enableLogsSample               | Boolean          | &check;      |
| escalationMessage              | String           | &check;      |
| evaluationDelay                | Long             | &check;      |
| groupbySimpleMonitor           | Boolean          | &check;      |
| includeTags                    | Boolean          | &check;      |
| locked                         | Boolean          | &check;      |
| minFailureDuration             | Long             | &check;      |
| minLocationFailed              | Long             | &check;      |
| newGroupDelay                  | Long             | &check;      |
| newHostDelay                   | Long             | &check;      |
| noDataTimeframe                | Long             | &check;      |
| notifyAudit                    | Boolean          | &check;      |
| notifyNoData                   | Boolean          | &check;      |
| renotifyInterval               | Long             | &check;      |
| renotifyOccurrences            | Long             | &check;      |
| requireFullWindow              | Boolean          | &check;      |
| silenced                       | Map<String,Long> | &check;      |
| syntheticsCheckId              | String           | &check;      |
| thresholdWindowsRecoveryWindow | String           | &check;      |
| thresholdWindowsTriggerWindow  | String           | &check;      |
| thresholds                     | Thresholds       | &check;      |
| timeoutH                       | Long             | &check;      |
| variables                      | JSON             | &check;      |

#### StateGroup
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| lastNodataTs    | Long     | &check;      |
| lastNotifiedTs  | Long     | &check;      |
| lastResolvedTs  | Long     | &check;      |
| lastTriggeredTs | Long     | &check;      |
| name            | String   | &check;      |
| status          | Value    | &check;      |

#### Thresholds
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| critical         | Double   | &check;      |
| criticalRecovery | Double   | &check;      |
| ok               | Double   | &check;      |
| unknown          | Double   | &check;      |
| warning          | Double   | &check;      |
| warningRecovery  | Double   | &check;      |

#### Value
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| valid    | Boolean  | &check;      |
| value    | String   | &check;      |
