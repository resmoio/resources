---
description: Amazon Web Services RDS Event Subscription
---
aws_rds_event_subscription
--------------------------

| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| accountId                | String       | &cross;      |
| custSubscriptionId       | String       | &cross;      |
| customerAwsId            | String       | &cross;      |
| enabled                  | Boolean      | &check;      |
| eventCategoriesList      | List<String> | &check;      |
| eventSubscriptionArn     | String       | &check;      |
| region                   | String       | &cross;      |
| snsTopicArn              | String       | &check;      |
| sourceIdsList            | List<String> | &check;      |
| sourceType               | String       | &check;      |
| status                   | String       | &check;      |
| subscriptionCreationTime | String       | &check;      |
