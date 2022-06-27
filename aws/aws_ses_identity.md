---
description: Amazon Web Services SES Identity
---
aws_ses_identity
----------------

| **Name**                 | **Type**               | **Nullable** |
| ------------------------ | ---------------------- | ------------ |
| accountId                | String                 | &cross;      |
| configurationSetName     | String                 | &check;      |
| dkimAttributes           | DkimAttributes         | &check;      |
| feedbackForwardingStatus | Boolean                | &check;      |
| identityName             | String                 | &cross;      |
| identityType             | String                 | &check;      |
| mailFromAttributes       | MailFromAttributes     | &check;      |
| notificationAttributes   | NotificationAttributes | &check;      |
| policies                 | Map<String,String>     | &check;      |
| region                   | String                 | &cross;      |
| tags                     | Map<String,String>     | &check;      |
| verifiedForSendingStatus | Boolean                | &check;      |

#### DkimAttributes
| **Name**                   | **Type**     | **Nullable** |
| -------------------------- | ------------ | ------------ |
| currentSigningKeyLength    | String       | &check;      |
| lastKeyGenerationTimestamp | String       | &check;      |
| nextSigningKeyLength       | String       | &check;      |
| signingAttributesOrigin    | String       | &check;      |
| signingEnabled             | Boolean      | &check;      |
| status                     | String       | &check;      |
| tokens                     | List<String> | &check;      |

#### MailFromAttributes
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| behaviorOnMxFailure  | String   | &check;      |
| mailFromDomain       | String   | &check;      |
| mailFromDomainStatus | String   | &check;      |

#### NotificationAttributes
| **Name**                               | **Type** | **Nullable** |
| -------------------------------------- | -------- | ------------ |
| bounceTopic                            | String   | &check;      |
| complaintTopic                         | String   | &check;      |
| deliveryTopic                          | String   | &check;      |
| forwardingEnabled                      | Boolean  | &check;      |
| headersInBounceNotificationsEnabled    | Boolean  | &check;      |
| headersInComplaintNotificationsEnabled | Boolean  | &check;      |
| headersInDeliveryNotificationsEnabled  | Boolean  | &check;      |
