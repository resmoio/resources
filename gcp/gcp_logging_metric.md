---
description: Google Cloud Platform Logging Metric
---
gcp_logging_metric
------------------

| **Name**         | **Type**           | **Nullable** |
| ---------------- | ------------------ | ------------ |
| bucketOptions    | BucketOptions      | &check;      |
| createTime       | String             | &check;      |
| description      | String             | &check;      |
| disabled         | Boolean            | &check;      |
| filter           | String             | &check;      |
| labelExtractors  | Map<String,String> | &check;      |
| metricDescriptor | MetricDescriptor   | &check;      |
| name             | String             | &cross;      |
| project          | String             | &cross;      |
| updateTime       | String             | &check;      |
| valueExtractor   | String             | &check;      |
| version          | String             | &check;      |

#### BucketOptions
| **Name**           | **Type**                  | **Nullable** |
| ------------------ | ------------------------- | ------------ |
| explicitBuckets    | BucketOptions.Explicit    | &check;      |
| exponentialBuckets | BucketOptions.Exponential | &check;      |
| linearBuckets      | BucketOptions.Linear      | &check;      |

#### BucketOptions.Explicit
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| bounds   | List<Number> | &check;      |

#### BucketOptions.Exponential
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| growthFactor     | Number   | &check;      |
| numFiniteBuckets | Int      | &check;      |
| scale            | Number   | &check;      |

#### BucketOptions.Linear
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| numFiniteBuckets | Int      | &check;      |
| offset           | Number   | &check;      |
| width            | Number   | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### MetricDescriptor
| **Name**               | **Type**                               | **Nullable** |
| ---------------------- | -------------------------------------- | ------------ |
| description            | String                                 | &check;      |
| displayName            | String                                 | &check;      |
| labels                 | List<MetricDescriptor.LabelDescriptor> | &check;      |
| launchStage            | Int                                    | &check;      |
| metricKind             | String                                 | &check;      |
| monitoredResourceTypes | List<String>                           | &check;      |
| name                   | String                                 | &cross;      |
| type                   | String                                 | &cross;      |
| unit                   | String                                 | &check;      |
| valueType              | String                                 | &check;      |

#### MetricDescriptor.LabelDescriptor
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| key         | String   | &check;      |
| valueType   | String   | &check;      |
