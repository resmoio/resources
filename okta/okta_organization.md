---
description: Okta Organization
---
okta_organization
-----------------

| **Name**                | **Type**                       | **Nullable** |
| ----------------------- | ------------------------------ | ------------ |
| clientPrivilegesSetting | ClientPrivilegesSetting        | &check;      |
| companyName             | String                         | &check;      |
| created                 | String                         | &check;      |
| endUserSupportHelpURL   | String                         | &check;      |
| expiresAt               | String                         | &check;      |
| id                      | String                         | &cross;      |
| lastUpdated             | String                         | &check;      |
| status                  | String                         | &check;      |
| subDomain               | String                         | &check;      |
| supportSetting          | OktaOrganizationSupportSetting | &check;      |
| website                 | String                         | &check;      |

#### ClientPrivilegesSetting
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| clientPrivilegesSetting | Boolean  | &check;      |

#### OktaOrganizationSupportSetting
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| expiration | String   | &check;      |
| support    | String   | &check;      |
