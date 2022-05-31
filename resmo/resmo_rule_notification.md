---
description: Resmo Rule Notification
---
resmo_rule_notification
-----------------------

| **Name**             | **Type**                               | **Nullable** |
| -------------------- | -------------------------------------- | ------------ |
| accountId            | String                                 | &check;      |
| createdAt            | Timestamp                              | &check;      |
| createdBy            | String                                 | &check;      |
| description          | String                                 | &check;      |
| id                   | String                                 | &cross;      |
| isEnabled            | Boolean                                | &check;      |
| name                 | String                                 | &check;      |
| notificationChannels | List<RuleNotificationChannelOptionDTO> | &check;      |
| severities           | List<String>                           | &check;      |
| tags                 | List<String>                           | &check;      |
| updatedAt            | Timestamp                              | &check;      |

#### RuleNotificationChannelOptionDTO
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
