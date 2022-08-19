---
description: Amazon Web Services Inspector Assessment Run
---
aws_inspector_assessment_run
----------------------------

| **Name**                  | **Type**                        | **Nullable** |
| ------------------------- | ------------------------------- | ------------ |
| accountId                 | String                          | &cross;      |
| accountName               | String                          | &check;      |
| arn                       | String                          | &cross;      |
| assessmentTemplateArn     | String                          | &check;      |
| completedAt               | String                          | &check;      |
| createdAt                 | String                          | &check;      |
| dataCollected             | Boolean                         | &check;      |
| durationInSeconds         | Int                             | &check;      |
| findingCounts             | Map<String,Int>                 | &check;      |
| name                      | String                          | &cross;      |
| notifications             | List<AssessmentRunNotification> | &check;      |
| rulesPackageArns          | List<String>                    | &check;      |
| startedAt                 | String                          | &check;      |
| state                     | String                          | &check;      |
| stateChangedAt            | String                          | &check;      |
| stateChanges              | List<AssessmentRunStateChange>  | &check;      |
| userAttributesForFindings | Map<String,String>              | &check;      |

#### AssessmentRunNotification
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| date                 | String   | &check;      |
| error                | Boolean  | &check;      |
| event                | String   | &check;      |
| message              | String   | &check;      |
| snsPublishStatusCode | String   | &check;      |
| snsTopicArn          | String   | &check;      |

#### AssessmentRunStateChange
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| state          | String   | &check;      |
| stateChangedAt | String   | &check;      |
