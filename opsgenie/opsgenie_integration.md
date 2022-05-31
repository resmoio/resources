---
description: Opsgenie Integration
---
opsgenie_integration
--------------------

| **Name**                    | **Type**        | **Nullable** |
| --------------------------- | --------------- | ------------ |
| accountName                 | String          | &check;      |
| alertActions                | List<String>    | &check;      |
| alertFilter                 | AlertFilter     | &check;      |
| allowConfigurationAccess    | Boolean         | &check;      |
| allowDeleteAccess           | Boolean         | &check;      |
| allowReadAccess             | Boolean         | &check;      |
| allowWriteAccess            | Boolean         | &check;      |
| enabled                     | Boolean         | &check;      |
| id                          | String          | &cross;      |
| ignoreRespondersFromPayload | Boolean         | &check;      |
| ignoreTeamsFromPayload      | Boolean         | &check;      |
| isAdvanced                  | Boolean         | &check;      |
| isGlobal                    | Boolean         | &check;      |
| name                        | String          | &cross;      |
| responders                  | List<Responder> | &check;      |
| sendAlertActions            | Boolean         | &check;      |
| suppressNotifications       | Boolean         | &check;      |
| type                        | String          | &check;      |

#### AlertFilter
| **Name**           | **Type**                    | **Nullable** |
| ------------------ | --------------------------- | ------------ |
| conditionMatchType | String                      | &check;      |
| conditions         | List<AlertFilter.Condition> | &check;      |

#### AlertFilter.Condition
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| expectedValue | String   | &check;      |
| field         | String   | &check;      |
| not           | Boolean  | &check;      |
| operation     | String   | &check;      |
| order         | Int      | &check;      |

#### Responder
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |
