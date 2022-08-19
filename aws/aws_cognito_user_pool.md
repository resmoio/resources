---
description: Amazon Web Services Cognito User Pool
---
aws_cognito_user_pool
---------------------

| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| accountId                   | String                      | &cross;      |
| accountName                 | String                      | &check;      |
| accountRecoverySetting      | AccountRecoverySetting      | &check;      |
| adminCreateUserConfig       | AdminCreateUserConfig       | &check;      |
| aliasAttributes             | List<String>                | &check;      |
| arn                         | String                      | &check;      |
| autoVerifiedAttributes      | List<String>                | &check;      |
| clients                     | List<Client>                | &check;      |
| creationDate                | String                      | &check;      |
| customDomain                | String                      | &check;      |
| deviceConfiguration         | DeviceConfiguration         | &check;      |
| domain                      | String                      | &check;      |
| emailConfiguration          | EmailConfiguration          | &check;      |
| emailConfigurationFailure   | String                      | &check;      |
| emailVerificationMessage    | String                      | &check;      |
| emailVerificationSubject    | String                      | &check;      |
| estimatedNumberOfUsers      | Int                         | &check;      |
| id                          | String                      | &cross;      |
| lambdaConfig                | LambdaConfig                | &check;      |
| lastModifiedDate            | String                      | &check;      |
| mfaConfiguration            | String                      | &check;      |
| name                        | String                      | &check;      |
| policies                    | UserPoolPolicy              | &check;      |
| providers                   | List<Provider>              | &check;      |
| region                      | String                      | &cross;      |
| resourceServers             | List<ResourceServer>        | &check;      |
| schemaAttributes            | List<SchemaAttribute>       | &check;      |
| smsAuthenticationMessage    | String                      | &check;      |
| smsConfiguration            | SmsConfiguration            | &check;      |
| smsConfigurationFailure     | String                      | &check;      |
| smsVerificationMessage      | String                      | &check;      |
| status                      | String                      | &check;      |
| userPoolAddOns              | UserPoolAddOns              | &check;      |
| userPoolTags                | Map<String,String>          | &check;      |
| usernameAttributes          | List<String>                | &check;      |
| usernameConfiguration       | UsernameConfiguration       | &check;      |
| verificationMessageTemplate | VerificationMessageTemplate | &check;      |

#### AccountRecoverySetting
| **Name**           | **Type**             | **Nullable** |
| ------------------ | -------------------- | ------------ |
| recoveryMechanisms | List<RecoveryOption> | &check;      |

#### AdminCreateUserConfig
| **Name**                  | **Type**        | **Nullable** |
| ------------------------- | --------------- | ------------ |
| allowAdminCreateUserOnly  | Boolean         | &check;      |
| inviteMessageTemplate     | MessageTemplate | &check;      |
| unusedAccountValidityDays | Int             | &check;      |

#### Client
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| clientId   | String   | &check;      |
| clientName | String   | &check;      |

#### CustomEmailLambdaVersionConfig
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| lambdaArn     | String   | &check;      |
| lambdaVersion | String   | &check;      |

#### CustomSMSLambdaVersionConfig
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| lambdaArn     | String   | &cross;      |
| lambdaVersion | String   | &cross;      |

#### DeviceConfiguration
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| challengeRequiredOnNewDevice     | Boolean  | &check;      |
| deviceOnlyRememberedOnUserPrompt | Boolean  | &check;      |

#### EmailConfiguration
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| configurationSet    | String   | &check;      |
| emailSendingAccount | String   | &check;      |
| from                | String   | &check;      |
| replyToEmailAddress | String   | &check;      |
| sourceArn           | String   | &check;      |

#### LambdaConfig
| **Name**                    | **Type**                       | **Nullable** |
| --------------------------- | ------------------------------ | ------------ |
| createAuthChallenge         | String                         | &check;      |
| customEmailSender           | CustomEmailLambdaVersionConfig | &check;      |
| customMessage               | String                         | &check;      |
| customSMSSender             | CustomSMSLambdaVersionConfig   | &check;      |
| defineAuthChallenge         | String                         | &check;      |
| kmsKeyID                    | String                         | &check;      |
| postAuthentication          | String                         | &check;      |
| postConfirmation            | String                         | &check;      |
| preAuthentication           | String                         | &check;      |
| preSignUp                   | String                         | &check;      |
| preTokenGeneration          | String                         | &check;      |
| userMigration               | String                         | &check;      |
| verifyAuthChallengeResponse | String                         | &check;      |

#### MessageTemplate
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| emailMessage | String   | &check;      |
| emailSubject | String   | &check;      |
| smsMessage   | String   | &check;      |

#### NumberAttributeConstraints
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| maxValue | String   | &check;      |
| minValue | String   | &check;      |

#### PasswordPolicy
| **Name**                      | **Type** | **Nullable** |
| ----------------------------- | -------- | ------------ |
| minimumLength                 | Int      | &check;      |
| requireLowercase              | Boolean  | &check;      |
| requireNumbers                | Boolean  | &check;      |
| requireSymbols                | Boolean  | &check;      |
| requireUppercase              | Boolean  | &check;      |
| temporaryPasswordValidityDays | Int      | &check;      |

#### Provider
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| creationDate     | String   | &check;      |
| lastModifiedDate | String   | &check;      |
| providerName     | String   | &check;      |
| providerType     | String   | &check;      |

#### RecoveryOption
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| priority | Int      | &check;      |

#### ResourceServer
| **Name**   | **Type**                  | **Nullable** |
| ---------- | ------------------------- | ------------ |
| identifier | String                    | &check;      |
| name       | String                    | &check;      |
| scopes     | List<ResourceServerScope> | &check;      |

#### ResourceServerScope
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| scopeDescription | String   | &check;      |
| scopeName        | String   | &check;      |

#### SchemaAttribute
| **Name**                   | **Type**                   | **Nullable** |
| -------------------------- | -------------------------- | ------------ |
| attributeDataType          | String                     | &check;      |
| developerOnlyAttribute     | Boolean                    | &check;      |
| mutable                    | Boolean                    | &check;      |
| name                       | String                     | &check;      |
| numberAttributeConstraints | NumberAttributeConstraints | &check;      |
| required                   | Boolean                    | &check;      |
| stringAttributeConstraints | StringAttributeConstraints | &check;      |

#### SmsConfiguration
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| externalId   | String   | &check;      |
| snsCallerArn | String   | &check;      |
| snsRegion    | String   | &check;      |

#### StringAttributeConstraints
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| maxLength | String   | &check;      |
| minLength | String   | &check;      |

#### UserPoolAddOns
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| advancedSecurityMode | String   | &check;      |

#### UserPoolPolicy
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| passwordPolicy | PasswordPolicy | &check;      |

#### UsernameConfiguration
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| caseSensitive | Boolean  | &check;      |

#### VerificationMessageTemplate
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| defaultEmailOption | String   | &check;      |
| emailMessage       | String   | &check;      |
| emailMessageByLink | String   | &check;      |
| emailSubject       | String   | &check;      |
| emailSubjectByLink | String   | &check;      |
| smsMessage         | String   | &check;      |
