---
description: Terraform Cloud Team
---
terraformcloud_team
-------------------

| **Name**           | **Type**            | **Nullable** |
| ------------------ | ------------------- | ------------ |
| id                 | String              | &cross;      |
| name               | String              | &check;      |
| organization       | String              | &check;      |
| organizationAccess | Map<String,Boolean> | &check;      |
| permissions        | Map<String,Boolean> | &check;      |
| ssoTeamId          | String              | &check;      |
| type               | String              | &check;      |
| usersCount         | Int                 | &check;      |
| visibility         | String              | &check;      |
