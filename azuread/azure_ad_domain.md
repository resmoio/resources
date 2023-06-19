---
description: Azure Active Directory Domain
---
azure_ad_domain
---------------

| **Name**                         | **Type**                       | **Nullable** |
| -------------------------------- | ------------------------------ | ------------ |
| authenticationType               | String                         | &check;      |
| availabilityStatus               | String                         | &check;      |
| domainNameReferences             | List<DirectoryObject>          | &check;      |
| federationConfiguration          | List<InternalDomainFederation> | &check;      |
| id                               | String                         | &cross;      |
| isAdminManaged                   | Boolean                        | &check;      |
| isDefault                        | Boolean                        | &check;      |
| isInitial                        | Boolean                        | &check;      |
| isRoot                           | Boolean                        | &check;      |
| isVerified                       | Boolean                        | &check;      |
| manufacturer                     | String                         | &check;      |
| model                            | String                         | &check;      |
| oDataType                        | String                         | &check;      |
| passwordNotificationWindowInDays | Int                            | &check;      |
| passwordValidityPeriodInDays     | Int                            | &check;      |
| serviceConfigurationRecords      | List<DomainDnsRecord>          | &check;      |
| state                            | DomainState                    | &check;      |
| supportedServices                | List<String>                   | &check;      |
| verificationDnsRecords           | List<DomainDnsRecord>          | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |

#### DomainDnsRecord
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| id               | String   | &check;      |
| isOptional       | Boolean  | &check;      |
| label            | String   | &check;      |
| oDataType        | String   | &check;      |
| recordType       | String   | &check;      |
| supportedService | String   | &check;      |
| ttl              | Int      | &check;      |

#### DomainState
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| lastActionDateTime | String   | &check;      |
| oDataType          | String   | &check;      |
| operation          | String   | &check;      |
| status             | String   | &check;      |

#### InternalDomainFederation
| **Name**                              | **Type**                       | **Nullable** |
| ------------------------------------- | ------------------------------ | ------------ |
| activeSignInUri                       | String                         | &check;      |
| displayName                           | String                         | &check;      |
| federatedIdpMfaBehavior               | String                         | &check;      |
| id                                    | String                         | &check;      |
| isSignedAuthenticationRequestRequired | Boolean                        | &check;      |
| issuerUri                             | String                         | &check;      |
| metadataExchangeUri                   | String                         | &check;      |
| nextSigningCertificate                | String                         | &check;      |
| oDataType                             | String                         | &check;      |
| passiveSignInUri                      | String                         | &check;      |
| preferredAuthenticationProtocol       | String                         | &check;      |
| promptLoginBehavior                   | String                         | &check;      |
| signOutUri                            | String                         | &check;      |
| signingCertificate                    | String                         | &check;      |
| signingCertificateUpdateStatus        | SigningCertificateUpdateStatus | &check;      |

#### SigningCertificateUpdateStatus
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| certificateUpdateResult | String   | &check;      |
| id                      | String   | &check;      |
| lastRunDateTime         | String   | &check;      |
| oDataType               | String   | &check;      |
