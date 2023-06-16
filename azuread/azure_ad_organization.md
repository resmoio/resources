---
description: Azure Active Directory Organization
---
azure_ad_organization
---------------------

| **Name**                             | **Type**                                | **Nullable** |
| ------------------------------------ | --------------------------------------- | ------------ |
| assignedPlans                        | List<AssignedPlan>                      | &check;      |
| businessPhones                       | List<String>                            | &check;      |
| certificateBasedAuthConfiguration    | List<CertificateBasedAuthConfiguration> | &check;      |
| city                                 | String                                  | &check;      |
| country                              | String                                  | &check;      |
| countryLetterCode                    | String                                  | &check;      |
| createdDateTime                      | String                                  | &check;      |
| deletedDateTime                      | String                                  | &check;      |
| displayName                          | String                                  | &check;      |
| id                                   | String                                  | &cross;      |
| marketingNotificationEmails          | List<String>                            | &check;      |
| oDataType                            | String                                  | &check;      |
| onPremisesSyncEnabled                | Boolean                                 | &check;      |
| postalCode                           | String                                  | &check;      |
| preferredLanguage                    | String                                  | &check;      |
| privacyProfile                       | PrivacyProfile                          | &check;      |
| provisionedPlans                     | List<ProvisionedPlan>                   | &check;      |
| securityComplianceNotificationMails  | List<String>                            | &check;      |
| securityComplianceNotificationPhones | List<String>                            | &check;      |
| state                                | String                                  | &check;      |
| street                               | String                                  | &check;      |
| technicalNotificationMails           | List<String>                            | &check;      |
| tenantType                           | String                                  | &check;      |
| verifiedDomains                      | List<VerifiedDomain>                    | &check;      |

#### AssignedPlan
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| assignedDateTime | String   | &check;      |
| capabilityStatus | String   | &check;      |
| oDataType        | String   | &check;      |
| service          | String   | &check;      |
| servicePlanId    | String   | &check;      |

#### CertificateAuthority
| **Name**                          | **Type** | **Nullable** |
| --------------------------------- | -------- | ------------ |
| certificateRevocationListUrl      | String   | &check;      |
| deltaCertificateRevocationListUrl | String   | &check;      |
| isRootAuthority                   | Boolean  | &check;      |
| issuer                            | String   | &check;      |
| issuerSki                         | String   | &check;      |

#### CertificateBasedAuthConfiguration
| **Name**               | **Type**                   | **Nullable** |
| ---------------------- | -------------------------- | ------------ |
| certificateAuthorities | List<CertificateAuthority> | &cross;      |

#### PrivacyProfile
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| contactEmail | String   | &check;      |
| oDataType    | String   | &check;      |
| statementUrl | String   | &check;      |

#### ProvisionedPlan
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| capabilityStatus   | String   | &check;      |
| oDataType          | String   | &check;      |
| provisioningStatus | String   | &check;      |
| service            | String   | &check;      |

#### VerifiedDomain
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| capabilities | String   | &check;      |
| isDefault    | Boolean  | &check;      |
| isInitial    | Boolean  | &check;      |
| name         | String   | &check;      |
| oDataType    | String   | &check;      |
| type         | String   | &check;      |
