---
description: Google Cloud Platform Monitoring Alert Policy
---
gcp_monitoring_alert_policy
---------------------------

| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| alertStrategy        | AlertStrategy      | &check;      |
| combiner             | String             | &check;      |
| conditions           | List<Condition>    | &check;      |
| creationRecord       | MutationRecord     | &check;      |
| displayName          | String             | &check;      |
| documentation        | Documentation      | &check;      |
| enabled              | Boolean            | &check;      |
| mutationRecord       | MutationRecord     | &check;      |
| name                 | String             | &cross;      |
| notificationChannels | List<String>       | &check;      |
| project              | String             | &cross;      |
| userLabels           | Map<String,String> | &check;      |
| validity             | Status             | &check;      |

#### Aggregation
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| alignmentPeriod    | String       | &check;      |
| crossSeriesReducer | String       | &check;      |
| groupByFields      | List<String> | &check;      |
| perSeriesAligner   | String       | &check;      |

#### AlertStrategy
| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| autoClose             | String                | &check;      |
| notificationRateLimit | NotificationRateLimit | &check;      |

#### Condition
| **Name**                         | **Type**                         | **Nullable** |
| -------------------------------- | -------------------------------- | ------------ |
| conditionAbsent                  | MetricAbsence                    | &check;      |
| conditionMatchedLog              | LogMatch                         | &check;      |
| conditionMonitoringQueryLanguage | MonitoringQueryLanguageCondition | &check;      |
| conditionThreshold               | MetricThreshold                  | &check;      |
| displayName                      | String                           | &check;      |
| name                             | String                           | &check;      |

#### Documentation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| content  | String   | &check;      |
| mimeType | String   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### LogMatch
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| filter          | String             | &check;      |
| labelExtractors | Map<String,String> | &check;      |

#### MetricAbsence
| **Name**     | **Type**          | **Nullable** |
| ------------ | ----------------- | ------------ |
| aggregations | List<Aggregation> | &check;      |
| duration     | String            | &check;      |
| filter       | String            | &check;      |
| trigger      | Trigger           | &check;      |

#### MetricThreshold
| **Name**                | **Type**          | **Nullable** |
| ----------------------- | ----------------- | ------------ |
| aggregations            | List<Aggregation> | &check;      |
| comparison              | String            | &check;      |
| denominatorAggregations | List<Aggregation> | &check;      |
| denominatorFilter       | String            | &check;      |
| duration                | String            | &check;      |
| evaluationMissingData   | String            | &check;      |
| filter                  | String            | &check;      |
| thresholdValue          | Double            | &check;      |
| trigger                 | Trigger           | &check;      |

#### MonitoringQueryLanguageCondition
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| duration              | String   | &check;      |
| evaluationMissingData | String   | &check;      |
| query                 | String   | &check;      |
| trigger               | Trigger  | &check;      |

#### MutationRecord
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| mutateTime | String   | &check;      |
| mutatedBy  | String   | &check;      |

#### NotificationRateLimit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| period   | String   | &check;      |

#### Status
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| code     | Int      | &check;      |
| message  | String   | &check;      |

#### Trigger
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| count    | Int      | &check;      |
| percent  | Double   | &check;      |
