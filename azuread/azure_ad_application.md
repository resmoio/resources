---
description: Azure Active Directory Application
---
azure_ad_application
--------------------

| **Name**                     | **Type**                          | **Nullable** |
| ---------------------------- | --------------------------------- | ------------ |
| addIns                       | List<AddIn>                       | &check;      |
| api                          | ApiApplication                    | &check;      |
| appId                        | String                            | &check;      |
| appManagementPolicies        | List<AppManagementPolicy>         | &check;      |
| appRoles                     | List<AppRole>                     | &check;      |
| applicationTemplateId        | String                            | &check;      |
| certification                | Certification                     | &check;      |
| createdDateTime              | String                            | &check;      |
| createdOnBehalfOf            | DirectoryObject                   | &check;      |
| defaultRedirectUri           | String                            | &check;      |
| description                  | String                            | &check;      |
| disabledByMicrosoftStatus    | String                            | &check;      |
| displayName                  | String                            | &check;      |
| extensionProperties          | List<ExtensionProperty>           | &check;      |
| federatedIdentityCredentials | List<FederatedIdentityCredential> | &check;      |
| groupMembershipClaims        | String                            | &check;      |
| homeRealmDiscoveryPolicies   | List<Policy>                      | &check;      |
| id                           | String                            | &cross;      |
| identifierUris               | List<String>                      | &check;      |
| info                         | InformationalUrl                  | &check;      |
| isDeviceOnlyAuthSupported    | Boolean                           | &check;      |
| isFallbackPublicClient       | Boolean                           | &check;      |
| keyCredentials               | List<KeyCredential>               | &check;      |
| notes                        | String                            | &check;      |
| oDataType                    | String                            | &check;      |
| oauth2RequirePostResponse    | Boolean                           | &check;      |
| optionalClaims               | OptionalClaims                    | &check;      |
| owners                       | List<DirectoryObject>             | &check;      |
| parentalControlSettings      | ParentalControlSettings           | &check;      |
| passwordCredentials          | List<PasswordCredential>          | &check;      |
| publicClient                 | PublicClientApplication           | &check;      |
| publisherDomain              | String                            | &check;      |
| requestSignatureVerification | RequestSignatureVerification      | &check;      |
| requiredResourceAccess       | List<RequiredResourceAccess>      | &check;      |
| samlMetadataUrl              | String                            | &check;      |
| serviceManagementReference   | String                            | &check;      |
| signInAudience               | String                            | &check;      |
| spa                          | SpaApplication                    | &check;      |
| tags                         | List<String>                      | &check;      |
| tokenEncryptionKeyId         | String                            | &check;      |
| tokenIssuancePolicies        | List<Policy>                      | &check;      |
| tokenLifetimePolicies        | List<Policy>                      | &check;      |
| verifiedPublisher            | VerifiedPublisher                 | &check;      |
| web                          | WebApplication                    | &check;      |

#### AddIn
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| id         | String   | &check;      |
| oDataType  | String   | &check;      |
| properties | JSON     | &check;      |
| type       | String   | &check;      |

#### ApiApplication
| **Name**                    | **Type**                       | **Nullable** |
| --------------------------- | ------------------------------ | ------------ |
| acceptMappedClaims          | Boolean                        | &check;      |
| knownClientApplications     | List<String>                   | &check;      |
| oDataType                   | String                         | &check;      |
| oauth2PermissionScopes      | List<PermissionScope>          | &check;      |
| preAuthorizedApplications   | List<PreAuthorizedApplication> | &check;      |
| requestedAccessTokenVersion | Int                            | &check;      |

#### AppManagementConfiguration
| **Name**            | **Type**                      | **Nullable** |
| ------------------- | ----------------------------- | ------------ |
| keyCredentials      | List<CredentialConfiguration> | &check;      |
| passwordCredentials | List<CredentialConfiguration> | &check;      |

#### AppManagementPolicy
| **Name**     | **Type**                   | **Nullable** |
| ------------ | -------------------------- | ------------ |
| description  | String                     | &check;      |
| displayName  | String                     | &check;      |
| id           | String                     | &cross;      |
| isEnabled    | Boolean                    | &check;      |
| oDataType    | String                     | &check;      |
| restrictions | AppManagementConfiguration | &check;      |

#### AppRole
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| allowedMemberTypes | List<String> | &check;      |
| description        | String       | &check;      |
| displayName        | String       | &check;      |
| id                 | String       | &check;      |
| isEnabled          | Boolean      | &check;      |
| oDataType          | String       | &check;      |
| origin             | String       | &check;      |
| value              | String       | &check;      |

#### Certification
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| certificationDetailsUrl         | String   | &check;      |
| certificationExpirationDateTime | String   | &check;      |
| isCertifiedByMicrosoft          | Boolean  | &check;      |
| isPublisherAttested             | Boolean  | &check;      |
| lastCertificationDateTime       | String   | &check;      |
| oDataType                       | String   | &check;      |

#### CredentialConfiguration
| **Name**                            | **Type** | **Nullable** |
| ----------------------------------- | -------- | ------------ |
| maxLifetime                         | String   | &check;      |
| restrictForAppsCreatedAfterDateTime | String   | &check;      |
| restrictionType                     | String   | &check;      |

#### DirectoryObject
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |

#### ExtensionProperty
| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| appDisplayName         | String       | &check;      |
| dataType               | String       | &check;      |
| id                     | String       | &cross;      |
| isSyncedFromOnPremises | Boolean      | &check;      |
| name                   | String       | &check;      |
| oDataType              | String       | &check;      |
| targetObjects          | List<String> | &check;      |

#### FederatedIdentityCredential
| **Name**    | **Type**     | **Nullable** |
| ----------- | ------------ | ------------ |
| audiences   | List<String> | &check;      |
| description | String       | &check;      |
| id          | String       | &cross;      |
| issuer      | String       | &check;      |
| name        | String       | &check;      |
| oDataType   | String       | &check;      |
| subject     | String       | &check;      |

#### ImplicitGrantSettings
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| enableAccessTokenIssuance | Boolean  | &check;      |
| enableIdTokenIssuance     | Boolean  | &check;      |
| oDataType                 | String   | &check;      |

#### InformationalUrl
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| logoUrl             | String   | &check;      |
| marketingUrl        | String   | &check;      |
| oDataType           | String   | &check;      |
| privacyStatementUrl | String   | &check;      |
| supportUrl          | String   | &check;      |
| termsOfServiceUrl   | String   | &check;      |

#### KeyCredential
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| customKeyIdentifier | String   | &check;      |
| displayName         | String   | &check;      |
| endDateTime         | String   | &check;      |
| key                 | String   | &check;      |
| keyId               | String   | &check;      |
| oDataType           | String   | &check;      |
| startDateTime       | String   | &check;      |
| type                | String   | &check;      |
| usage               | String   | &check;      |

#### OptionalClaim
| **Name**             | **Type**     | **Nullable** |
| -------------------- | ------------ | ------------ |
| additionalProperties | List<String> | &check;      |
| essential            | Boolean      | &check;      |
| name                 | String       | &check;      |
| oDataType            | String       | &check;      |
| source               | String       | &check;      |

#### OptionalClaims
| **Name**    | **Type**            | **Nullable** |
| ----------- | ------------------- | ------------ |
| accessToken | List<OptionalClaim> | &check;      |
| idToken     | List<OptionalClaim> | &check;      |
| oDataType   | String              | &check;      |
| saml2Token  | List<OptionalClaim> | &check;      |

#### ParentalControlSettings
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| countriesBlockedForMinors | List<String> | &check;      |
| legalAgeGroupRule         | String       | &check;      |
| oDataType                 | String       | &check;      |

#### PasswordCredential
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| displayName   | String   | &check;      |
| endDateTime   | String   | &check;      |
| hint          | String   | &check;      |
| keyId         | String   | &check;      |
| oDataType     | String   | &check;      |
| secretText    | String   | &check;      |
| startDateTime | String   | &check;      |

#### PermissionScope
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| adminConsentDescription | String   | &check;      |
| adminConsentDisplayName | String   | &check;      |
| id                      | String   | &check;      |
| isEnabled               | Boolean  | &check;      |
| oDataType               | String   | &check;      |
| origin                  | String   | &check;      |
| type                    | String   | &check;      |
| userConsentDescription  | String   | &check;      |
| userConsentDisplayName  | String   | &check;      |
| value                   | String   | &check;      |

#### Policy
| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| definition            | List<String> | &check;      |
| deletedDateTime       | String       | &check;      |
| description           | String       | &check;      |
| displayName           | String       | &check;      |
| id                    | String       | &check;      |
| isEnabled             | Boolean      | &check;      |
| isOrganizationDefault | Boolean      | &check;      |
| oDataType             | String       | &check;      |

#### PreAuthorizedApplication
| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| appId                  | String       | &check;      |
| delegatedPermissionIds | List<String> | &check;      |
| oDataType              | String       | &check;      |

#### PublicClientApplication
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| oDataType    | String       | &check;      |
| redirectUris | List<String> | &check;      |

#### RedirectUriSettings
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| index     | Int      | &check;      |
| oDataType | String   | &check;      |
| uri       | String   | &check;      |

#### RequestSignatureVerification
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| allowedWeakAlgorithms   | List<String> | &check;      |
| isSignedRequestRequired | Boolean      | &check;      |
| oDataType               | String       | &check;      |

#### RequiredResourceAccess
| **Name**       | **Type**             | **Nullable** |
| -------------- | -------------------- | ------------ |
| oDataType      | String               | &check;      |
| resourceAccess | List<ResourceAccess> | &check;      |
| resourceAppId  | String               | &check;      |

#### ResourceAccess
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| oDataType | String   | &check;      |
| type      | String   | &check;      |

#### SpaApplication
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| oDataType    | String       | &check;      |
| redirectUris | List<String> | &check;      |

#### VerifiedPublisher
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| addedDateTime       | String   | &check;      |
| displayName         | String   | &check;      |
| oDataType           | String   | &check;      |
| verifiedPublisherId | String   | &check;      |

#### WebApplication
| **Name**              | **Type**                  | **Nullable** |
| --------------------- | ------------------------- | ------------ |
| homePageUrl           | String                    | &check;      |
| implicitGrantSettings | ImplicitGrantSettings     | &check;      |
| logoutUrl             | String                    | &check;      |
| oDataType             | String                    | &check;      |
| redirectUriSettings   | List<RedirectUriSettings> | &check;      |
| redirectUris          | List<String>              | &check;      |
