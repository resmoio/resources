---
description: Entity Object Storage
---
object_storage
--------------

| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| backupEnabled   | Boolean  | &check;      |
| backupRetention | Long     | &check;      |
| encrypted       | Boolean  | &check;      |
| isEu            | Boolean  | &check;      |
| name            | String   | &cross;      |
| referencedType  | String   | &cross;      |
| region          | String   | &check;      |

#### BasicResource
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| referencedType | String   | &cross;      |
