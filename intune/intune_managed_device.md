---
description: Intune Managed Device
---
intune_managed_device
---------------------

| **Name**                                  | **Type**                                  | **Nullable** |
| ----------------------------------------- | ----------------------------------------- | ------------ |
| activationLockBypassCode                  | String                                    | &check;      |
| androidSecurityPatchLevel                 | String                                    | &check;      |
| azureADDeviceId                           | String                                    | &check;      |
| azureADRegistered                         | Boolean                                   | &check;      |
| complianceGracePeriodExpirationDateTime   | String                                    | &check;      |
| complianceState                           | String                                    | &check;      |
| configurationManagerClientEnabledFeatures | ConfigurationManagerClientEnabledFeatures | &check;      |
| deviceActionResults                       | List<DeviceActionResult>                  | &check;      |
| deviceCategory                            | DeviceCategory                            | &check;      |
| deviceCategoryDisplayName                 | String                                    | &check;      |
| deviceCompliancePolicyStates              | List<DeviceCompliancePolicyState>         | &check;      |
| deviceConfigurationStates                 | List<DeviceConfigurationState>            | &check;      |
| deviceEnrollmentType                      | String                                    | &check;      |
| deviceHealthAttestationState              | DeviceHealthAttestationState              | &check;      |
| deviceName                                | String                                    | &check;      |
| deviceRegistrationState                   | String                                    | &check;      |
| easActivated                              | Boolean                                   | &check;      |
| easActivationDateTime                     | String                                    | &check;      |
| easDeviceId                               | String                                    | &check;      |
| emailAddress                              | String                                    | &check;      |
| enrolledDateTime                          | String                                    | &check;      |
| ethernetMacAddress                        | String                                    | &check;      |
| exchangeAccessState                       | String                                    | &check;      |
| exchangeAccessStateReason                 | String                                    | &check;      |
| exchangeLastSuccessfulSyncDateTime        | String                                    | &check;      |
| freeStorageSpaceInBytes                   | Long                                      | &check;      |
| iccid                                     | String                                    | &check;      |
| id                                        | String                                    | &cross;      |
| imei                                      | String                                    | &check;      |
| isEncrypted                               | Boolean                                   | &check;      |
| isSupervised                              | Boolean                                   | &check;      |
| jailBroken                                | String                                    | &check;      |
| lastSyncDateTime                          | String                                    | &check;      |
| managedDeviceName                         | String                                    | &check;      |
| managedDeviceOwnerType                    | String                                    | &check;      |
| managementAgent                           | String                                    | &check;      |
| manufacturer                              | String                                    | &check;      |
| meid                                      | String                                    | &check;      |
| model                                     | String                                    | &check;      |
| notes                                     | String                                    | &check;      |
| operatingSystem                           | String                                    | &check;      |
| osVersion                                 | String                                    | &check;      |
| partnerReportedThreatState                | String                                    | &check;      |
| phoneNumber                               | String                                    | &check;      |
| physicalMemoryInBytes                     | Long                                      | &check;      |
| remoteAssistanceSessionErrorDetails       | String                                    | &check;      |
| remoteAssistanceSessionUrl                | String                                    | &check;      |
| serialNumber                              | String                                    | &check;      |
| subscriberCarrier                         | String                                    | &check;      |
| totalStorageSpaceInBytes                  | Long                                      | &check;      |
| udid                                      | String                                    | &check;      |
| userDisplayName                           | String                                    | &check;      |
| userId                                    | String                                    | &check;      |
| userPrincipalName                         | String                                    | &check;      |
| wiFiMacAddress                            | String                                    | &check;      |

#### ConfigurationManagerClientEnabledFeatures
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| compliancePolicy         | Boolean  | &check;      |
| deviceConfiguration      | Boolean  | &check;      |
| inventory                | Boolean  | &check;      |
| modernApps               | Boolean  | &check;      |
| oDataType                | String   | &check;      |
| resourceAccess           | Boolean  | &check;      |
| windowsUpdateForBusiness | Boolean  | &check;      |

#### DeviceActionResult
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| actionName          | String   | &check;      |
| actionState         | String   | &check;      |
| lastUpdatedDateTime | String   | &check;      |
| oDataType           | String   | &check;      |
| startDateTime       | String   | &check;      |

#### DeviceCategory
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| displayName | String   | &check;      |
| id          | String   | &cross;      |

#### DeviceCompliancePolicySettingState
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| currentValue        | String              | &check;      |
| errorCode           | Long                | &check;      |
| errorDescription    | String              | &check;      |
| instanceDisplayName | String              | &check;      |
| oDataType           | String              | &check;      |
| setting             | String              | &check;      |
| settingName         | String              | &check;      |
| sources             | List<SettingSource> | &check;      |
| state               | String              | &check;      |
| userEmail           | String              | &check;      |
| userId              | String              | &check;      |
| userName            | String              | &check;      |
| userPrincipalName   | String              | &check;      |

#### DeviceCompliancePolicyState
| **Name**      | **Type**                                 | **Nullable** |
| ------------- | ---------------------------------------- | ------------ |
| displayName   | String                                   | &check;      |
| id            | String                                   | &cross;      |
| platformType  | String                                   | &check;      |
| settingCount  | Int                                      | &check;      |
| settingStates | List<DeviceCompliancePolicySettingState> | &check;      |
| state         | String                                   | &check;      |
| version       | Int                                      | &check;      |

#### DeviceConfigurationSettingState
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| currentValue        | String              | &check;      |
| errorCode           | Long                | &check;      |
| errorDescription    | String              | &check;      |
| id                  | String              | &cross;      |
| instanceDisplayName | String              | &check;      |
| oDataType           | String              | &check;      |
| setting             | String              | &check;      |
| settingName         | String              | &check;      |
| sources             | List<SettingSource> | &check;      |
| state               | String              | &check;      |
| userEmail           | String              | &check;      |
| userId              | String              | &check;      |
| userName            | String              | &check;      |
| userPrincipalName   | String              | &check;      |

#### DeviceConfigurationState
| **Name**      | **Type**                              | **Nullable** |
| ------------- | ------------------------------------- | ------------ |
| displayName   | String                                | &check;      |
| id            | String                                | &cross;      |
| platformType  | String                                | &check;      |
| settingCount  | Int                                   | &check;      |
| settingStates | List<DeviceConfigurationSettingState> | &check;      |
| state         | String                                | &check;      |
| version       | Int                                   | &check;      |

#### DeviceHealthAttestationState
| **Name**                                 | **Type** | **Nullable** |
| ---------------------------------------- | -------- | ------------ |
| attestationIdentityKey                   | String   | &check;      |
| bitLockerStatus                          | String   | &check;      |
| bootAppSecurityVersion                   | String   | &check;      |
| bootDebugging                            | String   | &check;      |
| bootManagerSecurityVersion               | String   | &check;      |
| bootManagerVersion                       | String   | &check;      |
| bootRevisionListInfo                     | String   | &check;      |
| codeIntegrity                            | String   | &check;      |
| codeIntegrityCheckVersion                | String   | &check;      |
| codeIntegrityPolicy                      | String   | &check;      |
| contentNamespaceUrl                      | String   | &check;      |
| contentVersion                           | String   | &check;      |
| dataExcutionPolicy                       | String   | &check;      |
| deviceHealthAttestationStatus            | String   | &check;      |
| earlyLaunchAntiMalwareDriverProtection   | String   | &check;      |
| healthAttestationSupportedStatus         | String   | &check;      |
| healthStatusMismatchInfo                 | String   | &check;      |
| issuedDateTime                           | String   | &check;      |
| lastUpdateDateTime                       | String   | &check;      |
| oDataType                                | String   | &check;      |
| operatingSystemKernelDebugging           | String   | &check;      |
| operatingSystemRevListInfo               | String   | &check;      |
| pcr0                                     | String   | &check;      |
| pcrHashAlgorithm                         | String   | &check;      |
| resetCount                               | Long     | &check;      |
| restartCount                             | Long     | &check;      |
| safeMode                                 | String   | &check;      |
| secureBoot                               | String   | &check;      |
| secureBootConfigurationPolicyFingerPrint | String   | &check;      |
| testSigning                              | String   | &check;      |
| tpmVersion                               | String   | &check;      |
| virtualSecureMode                        | String   | &check;      |
| windowsPE                                | String   | &check;      |

#### SettingSource
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| id          | String   | &check;      |
| oDataType   | String   | &check;      |
| sourceType  | String   | &check;      |
