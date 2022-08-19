---
description: Amazon Web Services Backup Report Job
---
aws_backup_report_job
---------------------

| **Name**          | **Type**          | **Nullable** |
| ----------------- | ----------------- | ------------ |
| accountId         | String            | &cross;      |
| accountName       | String            | &check;      |
| completionTime    | String            | &check;      |
| creationTime      | String            | &check;      |
| id                | String            | &cross;      |
| region            | String            | &cross;      |
| reportDestination | ReportDestination | &check;      |
| reportPlanArn     | String            | &cross;      |
| reportTemplate    | String            | &cross;      |
| status            | String            | &cross;      |
| statusMessage     | String            | &check;      |

#### ReportDestination
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| s3BucketName | String       | &cross;      |
| s3Keys       | List<String> | &cross;      |
