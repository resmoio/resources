---
description: Google Workspace Domain
---
gsuite_domain
-------------

| **Name**      | **Type**          | **Nullable** |
| ------------- | ----------------- | ------------ |
| creationTime  | Date              | &check;      |
| customerId    | String            | &cross;      |
| domainAliases | List<DomainAlias> | &check;      |
| domainName    | String            | &cross;      |
| isPrimary     | Boolean           | &check;      |
| verified      | Boolean           | &check;      |

#### DomainAlias
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| creationTime     | Date     | &cross;      |
| domainAliasName  | String   | &cross;      |
| parentDomainName | String   | &cross;      |
| verified         | Boolean  | &cross;      |
