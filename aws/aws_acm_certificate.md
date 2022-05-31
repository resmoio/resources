---
description: Amazon Web Services ACM Certificate
---
aws_acm_certificate
-------------------

| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| accountId               | String       | &cross;      |
| certificateArn          | String       | &cross;      |
| certificateAuthorityArn | String       | &check;      |
| createdAt               | String       | &check;      |
| domainName              | String       | &cross;      |
| extendedKeyUsages       | List<String> | &check;      |
| failureReason           | String       | &check;      |
| importedAt              | String       | &check;      |
| inUseBy                 | List<String> | &check;      |
| issuedAt                | String       | &check;      |
| issuer                  | String       | &check;      |
| keyAlgorithm            | String       | &cross;      |
| keyUsages               | List<String> | &check;      |
| notAfter                | String       | &check;      |
| notBefore               | String       | &check;      |
| options                 | String       | &check;      |
| region                  | String       | &cross;      |
| renewalEligibility      | String       | &cross;      |
| revocationReason        | String       | &check;      |
| revokedAt               | String       | &check;      |
| serial                  | String       | &check;      |
| signatureAlgorithm      | String       | &cross;      |
| status                  | String       | &cross;      |
| subject                 | String       | &check;      |
| subjectAlternativeNames | List<String> | &check;      |
| type                    | String       | &cross;      |
