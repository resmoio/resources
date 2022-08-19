---
description: Amazon Web Services GuardDuty Publishing Destination
---
aws_guardduty_publishing_destination
------------------------------------

| **Name**                        | **Type**              | **Nullable** |
| ------------------------------- | --------------------- | ------------ |
| accountId                       | String                | &cross;      |
| accountName                     | String                | &check;      |
| destinationId                   | String                | &cross;      |
| destinationProperties           | DestinationProperties | &check;      |
| destinationType                 | String                | &check;      |
| detectorId                      | String                | &cross;      |
| publishingFailureStartTimestamp | Long                  | &check;      |
| status                          | String                | &check;      |

#### DestinationProperties
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| destinationArn | String   | &cross;      |
| kmsKeyArn      | String   | &cross;      |
