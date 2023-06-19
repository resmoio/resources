---
description: Azure Active Directory Role Management Policy Assignment
---
azure_ad_role_management_policy_assignment
------------------------------------------

| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| id               | String   | &cross;      |
| oDataType        | String   | &check;      |
| policy           | Policy   | &check;      |
| policyId         | String   | &check;      |
| roleDefinitionId | String   | &check;      |
| scopeId          | String   | &check;      |
| scopeType        | String   | &check;      |

#### Identity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |
| oDataType   | String   | &check;      |

#### Policy
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| description           | String   | &check;      |
| displayName           | String   | &check;      |
| id                    | String   | &check;      |
| isOrganizationDefault | Boolean  | &check;      |
| oDataType             | String   | &check;      |
| scopeId               | String   | &check;      |
| scopeType             | String   | &check;      |
