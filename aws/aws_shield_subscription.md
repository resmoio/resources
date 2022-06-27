---
description: Amazon Web Services Shield Subscription
---
aws_shield_subscription
-----------------------

| **Name**                  | **Type**           | **Nullable** |
| ------------------------- | ------------------ | ------------ |
| accountId                 | String             | &cross;      |
| arn                       | String             | &cross;      |
| autoRenew                 | String             | &check;      |
| endTime                   | String             | &check;      |
| limits                    | Map<String,Long>   | &check;      |
| proactiveEngagementStatus | String             | &check;      |
| startTime                 | String             | &check;      |
| subscriptionLimits        | SubscriptionLimits | &check;      |
| timeCommitmentInSeconds   | Long               | &check;      |

#### ProtectionGroupArbitraryPatternLimits
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| maxMembers | Long     | &check;      |

#### ProtectionGroupLimits
| **Name**            | **Type**                         | **Nullable** |
| ------------------- | -------------------------------- | ------------ |
| maxProtectionGroups | Long                             | &check;      |
| patternTypeLimits   | ProtectionGroupPatternTypeLimits | &check;      |

#### ProtectionGroupPatternTypeLimits
| **Name**               | **Type**                              | **Nullable** |
| ---------------------- | ------------------------------------- | ------------ |
| arbitraryPatternLimits | ProtectionGroupArbitraryPatternLimits | &check;      |

#### ProtectionLimits
| **Name**                    | **Type**         | **Nullable** |
| --------------------------- | ---------------- | ------------ |
| protectedResourceTypeLimits | Map<String,Long> | &check;      |

#### SubscriptionLimits
| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| protectionGroupLimits | ProtectionGroupLimits | &check;      |
| protectionLimits      | ProtectionLimits      | &check;      |
