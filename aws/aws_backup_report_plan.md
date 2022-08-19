---
description: Amazon Web Services Backup Report Plan
---
aws_backup_report_plan
----------------------

| **Name**                    | **Type**              | **Nullable** |
| --------------------------- | --------------------- | ------------ |
| accountId                   | String                | &cross;      |
| accountName                 | String                | &check;      |
| arn                         | String                | &cross;      |
| creationTime                | String                | &check;      |
| deliveryChannel             | ReportDeliveryChannel | &check;      |
| deploymentStatus            | String                | &cross;      |
| description                 | String                | &cross;      |
| lastAttemptedExecutionTime  | String                | &check;      |
| lastSuccessfulExecutionTime | String                | &check;      |
| name                        | String                | &cross;      |
| region                      | String                | &cross;      |
| setting                     | ReportSetting         | &check;      |

#### ReportDeliveryChannel
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| formats      | List<String> | &check;      |
| s3BucketName | String       | &cross;      |
| s3KeyPrefix  | String       | &cross;      |

#### ReportSetting
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| frameworkArns      | List<String> | &cross;      |
| numberOfFrameworks | Int          | &cross;      |
| reportTemplate     | String       | &cross;      |
