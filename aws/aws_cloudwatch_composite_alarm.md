---
description: Amazon Web Services CloudWatch Composite Alarm
---
aws_cloudwatch_composite_alarm
------------------------------

| **Name**                           | **Type**     | **Nullable** |
| ---------------------------------- | ------------ | ------------ |
| accountId                          | String       | &cross;      |
| accountName                        | String       | &check;      |
| actionsEnabled                     | Boolean      | &check;      |
| alarmActions                       | List<String> | &check;      |
| alarmArn                           | String       | &cross;      |
| alarmConfigurationUpdatedTimestamp | String       | &check;      |
| alarmDescription                   | String       | &check;      |
| alarmName                          | String       | &cross;      |
| alarmRule                          | String       | &check;      |
| insufficientDataActions            | List<String> | &check;      |
| okActions                          | List<String> | &check;      |
| region                             | String       | &cross;      |
