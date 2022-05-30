---
description: Opsgenie Escalation
---
opsgenie_escalation
-------------------

| **Name**    | **Type**   | **Nullable** |
| ----------- | ---------- | ------------ |
| accountName | String     | &check;      |
| description | String     | &cross;      |
| id          | String     | &cross;      |
| name        | String     | &cross;      |
| repeat      | Repeat     | &check;      |
| rules       | List<Rule> | &check;      |

#### Repeat
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| closeAlertAfterAll   | Boolean  | &check;      |
| count                | Int      | &check;      |
| resetRecipientStates | Boolean  | &check;      |
| waitInterval         | Int      | &check;      |

#### Rule
| **Name**   | **Type**       | **Nullable** |
| ---------- | -------------- | ------------ |
| condition  | String         | &check;      |
| delay      | Rule.Delay     | &check;      |
| notifyType | String         | &check;      |
| recipient  | Rule.Recipient | &check;      |

#### Rule.Delay
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| timeAmount | Int      | &check;      |
| timeUnit   | String   | &check;      |

#### Rule.Recipient
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
| username | String   | &check;      |
