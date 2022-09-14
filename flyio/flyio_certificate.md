---
description: Flyio Certificate
---
flyio_certificate
-----------------

| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| appId                     | String       | &cross;      |
| appName                   | String       | &cross;      |
| certificateAuthority      | String       | &check;      |
| certificateRequestedAt    | String       | &check;      |
| check                     | Boolean      | &check;      |
| clientStatus              | String       | &check;      |
| createdAt                 | String       | &check;      |
| dnsProvider               | String       | &check;      |
| dnsValidationHostname     | String       | &check;      |
| dnsValidationInstructions | String       | &check;      |
| dnsValidationTarget       | String       | &check;      |
| domain                    | String       | &check;      |
| hostname                  | String       | &check;      |
| id                        | String       | &cross;      |
| isAcmeAlpnConfigured      | Boolean      | &check;      |
| isAcmeDnsConfigured       | Boolean      | &check;      |
| isApex                    | Boolean      | &check;      |
| isConfigured              | Boolean      | &check;      |
| isWildcard                | Boolean      | &check;      |
| issued                    | List<Issued> | &cross;      |
| source                    | String       | &check;      |

#### Issued
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| expiresAt | String   | &check;      |
| hostname  | String   | &check;      |
| id        | String   | &check;      |
| type      | String   | &check;      |
