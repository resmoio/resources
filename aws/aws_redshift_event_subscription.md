---
description: Amazon Web Services Redshift Event Subscription
---
aws_redshift_event_subscription
-------------------------------

| **Name**                 | **Type**           | **Nullable** |
| ------------------------ | ------------------ | ------------ |
| accountId                | String             | &cross;      |
| accountName              | String             | &check;      |
| custSubscriptionId       | String             | &cross;      |
| customerAwsId            | String             | &check;      |
| enabled                  | Boolean            | &check;      |
| eventCategoriesList      | List<String>       | &check;      |
| region                   | String             | &cross;      |
| severity                 | String             | &check;      |
| snsTopicArn              | String             | &check;      |
| sourceIdsList            | List<String>       | &check;      |
| sourceType               | String             | &check;      |
| status                   | String             | &check;      |
| subscriptionCreationTime | String             | &check;      |
| tags                     | Map<String,String> | &check;      |
