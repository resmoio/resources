---
description: Amazon Web Services KMS Grant
---
aws_kms_grant
-------------

| **Name**          | **Type**         | **Nullable** |
| ----------------- | ---------------- | ------------ |
| accountId         | String           | &cross;      |
| constraints       | GrantConstraints | &check;      |
| creationDate      | String           | &check;      |
| granteePrincipal  | String           | &cross;      |
| id                | String           | &cross;      |
| issuingAccount    | String           | &cross;      |
| keyId             | String           | &cross;      |
| name              | String           | &cross;      |
| operations        | List<String>     | &check;      |
| region            | String           | &cross;      |
| retiringPrincipal | String           | &check;      |

#### GrantConstraints
| **Name**                | **Type**           | **Nullable** |
| ----------------------- | ------------------ | ------------ |
| encryptionContextEquals | Map<String,String> | &check;      |
| encryptionContextSubset | Map<String,String> | &check;      |
