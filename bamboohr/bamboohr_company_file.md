---
description: BambooHR Company File
---
bamboohr_company_file
---------------------

| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| canDeleteFile      | String   | &check;      |
| canRenameFile      | String   | &check;      |
| category           | Category | &cross;      |
| createdBy          | String   | &check;      |
| dateCreated        | String   | &check;      |
| id                 | String   | &cross;      |
| name               | String   | &check;      |
| originalFileName   | String   | &check;      |
| shareWithEmployees | String   | &check;      |
| subdomain          | String   | &cross;      |

#### Category
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
