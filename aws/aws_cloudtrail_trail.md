---
description: Amazon Web Services CloudTrail
---
aws_cloudtrail_trail
--------------------

| **Name**                   | **Type**               | **Nullable** |
| -------------------------- | ---------------------- | ------------ |
| accountId                  | String                 | &cross;      |
| advancedSelectors          | List<AdvancedSelector> | &cross;      |
| cloudWatchLogsLogGroupArn  | String                 | &check;      |
| cloudWatchLogsRoleArn      | String                 | &check;      |
| eventSelectors             | List<EventSelector>    | &cross;      |
| hasCustomEventSelectors    | Boolean                | &check;      |
| hasInsightSelectors        | Boolean                | &check;      |
| homeRegion                 | String                 | &check;      |
| includeGlobalServiceEvents | Boolean                | &check;      |
| isMultiRegionTrail         | Boolean                | &check;      |
| isOrganizationTrail        | Boolean                | &check;      |
| kmsKeyId                   | String                 | &check;      |
| logFileValidationEnabled   | Boolean                | &check;      |
| name                       | String                 | &cross;      |
| region                     | String                 | &check;      |
| s3BucketName               | String                 | &check;      |
| s3KeyPrefix                | String                 | &check;      |
| snsTopicARN                | String                 | &check;      |
| trailARN                   | String                 | &cross;      |

#### AdvancedSelector
| **Name**       | **Type**                             | **Nullable** |
| -------------- | ------------------------------------ | ------------ |
| fieldSelectors | List<AdvancedSelector.FieldSelector> | &cross;      |
| name           | String                               | &cross;      |

#### AdvancedSelector.FieldSelector
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| endsWith      | List<String> | &check;      |
| equals        | List<String> | &check;      |
| field         | String       | &cross;      |
| notEndsWith   | List<String> | &check;      |
| notEquals     | List<String> | &check;      |
| notStartsWith | List<String> | &check;      |
| startsWith    | List<String> | &check;      |

#### EventSelector
| **Name**                      | **Type**                         | **Nullable** |
| ----------------------------- | -------------------------------- | ------------ |
| dataResources                 | List<EventSelector.DataResource> | &cross;      |
| excludeManagementEventSources | List<String>                     | &cross;      |
| includeManagementEvents       | Boolean                          | &cross;      |
| readWriteType                 | String                           | &cross;      |

#### EventSelector.DataResource
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| type     | String       | &cross;      |
| values   | List<String> | &cross;      |
