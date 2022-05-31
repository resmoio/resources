---
description: Amazon Web Services Backup Region Settings
---
aws_backup_region_settings
--------------------------

| **Name**                         | **Type**            | **Nullable** |
| -------------------------------- | ------------------- | ------------ |
| accountId                        | String              | &cross;      |
| region                           | String              | &cross;      |
| resourceTypeManagementPreference | Map<String,Boolean> | &check;      |
| resourceTypeOptInPreference      | Map<String,Boolean> | &check;      |
