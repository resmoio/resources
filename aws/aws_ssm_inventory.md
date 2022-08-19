---
description: Amazon Web Services SSM Inventory
---
aws_ssm_inventory
-----------------

| **Name**    | **Type**                       | **Nullable** |
| ----------- | ------------------------------ | ------------ |
| accountId   | String                         | &cross;      |
| accountName | String                         | &check;      |
| data        | List<InventoryItemInformation> | &check;      |
| id          | String                         | &cross;      |
| region      | String                         | &cross;      |

#### InventoryItemInformation
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| captureTime   | String   | &check;      |
| content       | JSON     | &check;      |
| schemaVersion | String   | &check;      |
| typeName      | String   | &check;      |
