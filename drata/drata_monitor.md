---
description: Drata Monitor
---
drata_monitor
-------------

| **Name**          | **Type**              | **Nullable** |
| ----------------- | --------------------- | ------------ |
| autoEnabledAt     | String                | &check;      |
| checkResultStatus | String                | &check;      |
| checkStatus       | String                | &check;      |
| controls          | List<Control>         | &check;      |
| createdAt         | String                | &check;      |
| description       | String                | &check;      |
| disabledMessage   | String                | &check;      |
| disablingUser     | String                | &check;      |
| id                | Long                  | &cross;      |
| lastCheck         | String                | &check;      |
| monitorInstances  | List<MonitorInstance> | &check;      |
| name              | String                | &check;      |
| priority          | String                | &check;      |
| testId            | String                | &check;      |

#### Control
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |

#### MonitorInstance
| **Name**                  | **Type**                                       | **Nullable** |
| ------------------------- | ---------------------------------------------- | ------------ |
| autopilotTaskType         | String                                         | &check;      |
| checkFrequency            | String                                         | &check;      |
| checkResultStatus         | String                                         | &check;      |
| createdAt                 | String                                         | &check;      |
| enabled                   | Boolean                                        | &check;      |
| failedTestDescription     | String                                         | &check;      |
| id                        | Long                                           | &check;      |
| monitorInstanceCheckTypes | List<MonitorInstance.MonitorInstanceCheckType> | &check;      |
| remedyDescription         | String                                         | &check;      |
| updatedAt                 | String                                         | &check;      |

#### MonitorInstance.MonitorInstanceCheckType
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| checkType | String   | &check;      |
| createdAt | String   | &check;      |
| id        | Long     | &check;      |
| updatedAt | String   | &check;      |
