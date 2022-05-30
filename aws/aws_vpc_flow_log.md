---
description: Amazon Web Services VPC Flow Log
---
aws_vpc_flow_log
----------------

| **Name**                 | **Type**           | **Nullable** |
| ------------------------ | ------------------ | ------------ |
| accountId                | String             | &cross;      |
| creationTime             | Long               | &check;      |
| deliverLogsErrorMessage  | String             | &check;      |
| deliverLogsPermissionArn | String             | &check;      |
| deliverLogsStatus        | String             | &check;      |
| destinationOptions       | DestinationOptions | &check;      |
| id                       | String             | &cross;      |
| logDestination           | String             | &check;      |
| logDestinationType       | String             | &check;      |
| logFormat                | String             | &check;      |
| logGroupName             | String             | &check;      |
| maxAggregationInterval   | Int                | &check;      |
| region                   | String             | &cross;      |
| resourceId               | String             | &check;      |
| status                   | String             | &check;      |
| tags                     | Map<String,String> | &check;      |
| trafficType              | String             | &check;      |

#### DestinationOptions
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| fileFormat               | String   | &check;      |
| hiveCompatiblePartitions | Boolean  | &check;      |
| perHourPartition         | Boolean  | &check;      |
