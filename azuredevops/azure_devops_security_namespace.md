---
description: Azure DevOps Security Namespace
---
azure_devops_security_namespace
-------------------------------

| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| accountId          | String       | &cross;      |
| accountName        | String       | &cross;      |
| actions            | List<Action> | &check;      |
| dataspaceCategory  | String       | &check;      |
| displayName        | String       | &check;      |
| elementLength      | Int          | &check;      |
| extensionType      | String       | &check;      |
| isRemotable        | Boolean      | &check;      |
| name               | String       | &check;      |
| namespaceId        | String       | &cross;      |
| readPermission     | Int          | &check;      |
| structureValue     | Int          | &check;      |
| systemBitMask      | Int          | &check;      |
| useTokenTranslator | Boolean      | &check;      |
| writePermission    | Int          | &check;      |

#### Action
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| bit         | Int      | &check;      |
| displayName | String   | &check;      |
| name        | String   | &check;      |
| namespaceId | String   | &check;      |
