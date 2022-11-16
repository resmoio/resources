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
| isEncrypted        | Boolean          | &check;      |
| owner              | String           | &check;      |
| ownerIsSharedDrive | Boolean          | &check;      |
| ownerIsTeamDrive   | Boolean          | &check;      |
| title              | String           | &check;      |
| type               | String           | &check;      |
| userAccess         | List<UserAccess> | &check;      |
| visibility         | Visibility       | &check;      |

#### UserAccess
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| scope    | String   | &check;      |
| user     | String   | &check;      |

#### Visibility
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| change       | String   | &check;      |
| scope        | String   | &check;      |
| targetDomain | String   | &check;      |
| type         | String   | &check;      |
