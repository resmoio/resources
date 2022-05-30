---
description: Amazon Web Services Config Recorder Status
---
aws_config_recorder_status
--------------------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| accountId      | String         | &cross;      |
| name           | String         | &cross;      |
| recordingGroup | RecordingGroup | &cross;      |
| region         | String         | &check;      |
| roleARN        | String         | &cross;      |
| status         | Status         | &check;      |

#### RecordingGroup
| **Name**                   | **Type**     | **Nullable** |
| -------------------------- | ------------ | ------------ |
| allSupported               | Boolean      | &cross;      |
| includeGlobalResourceTypes | Boolean      | &cross;      |
| resourceTypes              | List<String> | &cross;      |

#### Status
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| lastErrorCode    | String   | &check;      |
| lastErrorMessage | String   | &check;      |
| lastStartTime    | String   | &check;      |
| lastStatus       | String   | &check;      |
| lastStopTime     | String   | &check;      |
| name             | String   | &cross;      |
| recording        | Boolean  | &cross;      |
