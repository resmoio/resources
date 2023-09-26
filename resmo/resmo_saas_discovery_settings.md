---
description: Resmo Saas Discovery Settings
---
resmo_saas_discovery_settings
-----------------------------

| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| accountId                 | String       | &cross;      |
| createdAt                 | String       | &check;      |
| createdBy                 | String       | &check;      |
| directoryOnboardingNotify | TimeWithUnit | &check;      |
| extensionOnboardingNotify | TimeWithUnit | &check;      |
| inactiveTimeout           | Int          | &check;      |
| supportContact            | String       | &check;      |
| trackedDomains            | List<String> | &check;      |
| updatedAt                 | String       | &check;      |
| updatedBy                 | String       | &check;      |

#### TimeWithUnit
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| time     | Int      | &cross;      |
| unit     | String   | &cross;      |
