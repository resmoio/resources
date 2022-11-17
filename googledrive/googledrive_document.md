---
description: Google Drive Document
---
googledrive_document
--------------------

| **Name**           | **Type**         | **Nullable** |
| ------------------ | ---------------- | ------------ |
| createdAt          | Date             | &check;      |
| createdBy          | String           | &check;      |
| customerId         | String           | &cross;      |
| folderId           | String           | &check;      |
| id                 | String           | &cross;      |
| owner              | String           | &check;      |
| ownerIsSharedDrive | Boolean          | &check;      |
| title              | String           | &check;      |
| type               | String           | &check;      |
| userAccess         | List<UserAccess> | &cross;      |
| visibility         | Visibility       | &cross;      |

#### UserAccess
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| scope    | String   | &check;      |
| user     | String   | &check;      |

#### Visibility
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| change       | String   | &cross;      |
| changeAt     | Date     | &check;      |
| targetDomain | String   | &check;      |
| type         | String   | &cross;      |
