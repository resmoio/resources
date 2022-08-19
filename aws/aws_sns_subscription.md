---
description: Amazon Web Services SNS Subscription
---
aws_sns_subscription
--------------------

| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| accountId                    | String   | &cross;      |
| accountName                  | String   | &check;      |
| confirmationWasAuthenticated | Boolean  | &cross;      |
| endpoint                     | String   | &cross;      |
| filterPolicy                 | JSON     | &check;      |
| owner                        | String   | &cross;      |
| pendingConfirmation          | Boolean  | &cross;      |
| protocol                     | String   | &cross;      |
| rawMessageDelivery           | Boolean  | &cross;      |
| redrivePolicy                | JSON     | &check;      |
| region                       | String   | &cross;      |
| subscriptionArn              | String   | &cross;      |
| topicArn                     | String   | &cross;      |
