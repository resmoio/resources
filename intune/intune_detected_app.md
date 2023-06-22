---
description: Intune Detected App
---
intune_detected_app
-------------------

| **Name**       | **Type**            | **Nullable** |
| -------------- | ------------------- | ------------ |
| deviceCount    | Int                 | &check;      |
| displayName    | String              | &check;      |
| id             | String              | &cross;      |
| managedDevices | List<ManagedDevice> | &check;      |
| sizeInByte     | Long                | &check;      |
| version        | String              | &check;      |

#### ManagedDevice
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| deviceName | String   | &check;      |
| id         | String   | &cross;      |
