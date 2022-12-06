---
description: GoDaddy Domain
---
godaddy_domain
--------------

| **Name**               | **Type**           | **Nullable** |
| ---------------------- | ------------------ | ------------ |
| actions                | List<Action>       | &check;      |
| authCode               | String             | &check;      |
| createdAt              | String             | &check;      |
| deletedAt              | String             | &check;      |
| dnssecRecords          | List<Record>       | &check;      |
| domain                 | String             | &check;      |
| domainId               | String             | &cross;      |
| expirationProtected    | Boolean            | &check;      |
| expiresAt              | String             | &check;      |
| holdRegistrar          | Boolean            | &check;      |
| hostnames              | List<String>       | &check;      |
| locked                 | Boolean            | &check;      |
| modifiedAt             | String             | &check;      |
| nameServers            | List<String>       | &check;      |
| privacy                | Boolean            | &check;      |
| registrarCreatedAt     | String             | &check;      |
| registryStatusCodes    | List<String>       | &check;      |
| renewAuto              | Boolean            | &check;      |
| renewDeadline          | String             | &check;      |
| renewal                | Renewal            | &check;      |
| shopperId              | String             | &check;      |
| status                 | String             | &check;      |
| subaccountId           | String             | &check;      |
| transferAwayEligibleAt | String             | &check;      |
| transferProtected      | Boolean            | &check;      |
| verifications          | Map<String,String> | &check;      |

#### Action
| **Name**    | **Type**      | **Nullable** |
| ----------- | ------------- | ------------ |
| completedAt | String        | &check;      |
| createdAt   | String        | &check;      |
| modifiedAt  | String        | &check;      |
| origination | String        | &check;      |
| reason      | Action.Reason | &check;      |
| requestId   | String        | &check;      |
| startedAt   | String        | &check;      |
| status      | String        | &check;      |
| type        | String        | &check;      |

#### Action.Reason
| **Name** | **Type**  | **Nullable** |
| -------- | --------- | ------------ |
| code     | String    | &check;      |
| fields   | List<Map> | &check;      |
| message  | String    | &check;      |

#### Record
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| algorithm        | String   | &check;      |
| digest           | String   | &check;      |
| digestType       | String   | &check;      |
| flags            | String   | &check;      |
| keyTag           | Int      | &check;      |
| maxSignatureLife | Int      | &check;      |
| publicKey        | String   | &check;      |

#### Renewal
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| currency  | String   | &check;      |
| price     | Int      | &check;      |
| renewable | Boolean  | &check;      |
