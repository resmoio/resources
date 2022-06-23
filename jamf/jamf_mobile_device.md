---
description: Jamf Pro Mobile Device
---
jamf_mobile_device
------------------

| **Name**                           | **Type**                              | **Nullable** |
| ---------------------------------- | ------------------------------------- | ------------ |
| applications                       | List<Application>                     | &check;      |
| assetTag                           | String                                | &check;      |
| available                          | Int                                   | &check;      |
| bleCapable                         | Boolean                               | &check;      |
| bluetoothMacAddress                | String                                | &check;      |
| capacity                           | Int                                   | &check;      |
| certificates                       | List<Certificate>                     | &check;      |
| cloudBackupEnabled                 | Boolean                               | &check;      |
| configurationProfiles              | List<ConfigurationProfile>            | &check;      |
| deviceLocatorServiceEnabled        | Boolean                               | &check;      |
| deviceName                         | String                                | &check;      |
| deviceOwnershipLevel               | String                                | &check;      |
| displayName                        | String                                | &check;      |
| doNotDisturbEnabled                | Boolean                               | &check;      |
| exchangeActivesyncDeviceIdentifier | String                                | &check;      |
| extensionAttributes                | List<ExtensionAttribute>              | &check;      |
| id                                 | Int                                   | &cross;      |
| initialEntryDateUtc                | String                                | &check;      |
| ipAddress                          | String                                | &check;      |
| itunesStoreAccountIsActive         | Boolean                               | &check;      |
| lastBackupTimeUtc                  | String                                | &check;      |
| lastCloudBackupDateUtc             | String                                | &check;      |
| lastEnrollmentUtc                  | String                                | &check;      |
| lastInventoryUpdate                | String                                | &check;      |
| lastInventoryUpdateUtc             | String                                | &check;      |
| location                           | Location                              | &check;      |
| locationServicesEnabled            | Boolean                               | &check;      |
| managed                            | Boolean                               | &check;      |
| mobileDeviceGroups                 | List<MobileDeviceGroup>               | &check;      |
| model                              | String                                | &check;      |
| modelDisplay                       | String                                | &check;      |
| modelIdentifier                    | String                                | &check;      |
| modelNumber                        | String                                | &check;      |
| modemFirmware                      | String                                | &check;      |
| name                               | String                                | &check;      |
| network                            | Network                               | &check;      |
| osBuild                            | String                                | &check;      |
| osType                             | String                                | &check;      |
| osVersion                          | String                                | &check;      |
| phoneNumber                        | String                                | &check;      |
| provisioningProfiles               | List<MobileDeviceProvisioningProfile> | &check;      |
| purchasing                         | Purchasing                            | &check;      |
| securityObject                     | SecurityObject                        | &check;      |
| serialNumber                       | String                                | &check;      |
| serverName                         | String                                | &cross;      |
| shared                             | String                                | &check;      |
| supervised                         | Boolean                               | &check;      |
| tethered                           | String                                | &check;      |
| udid                               | String                                | &check;      |
| wifiMacAddress                     | String                                | &check;      |

#### Application
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| applicationName    | String   | &check;      |
| applicationVersion | String   | &check;      |
| identifier         | String   | &check;      |

#### Certificate
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| commonName | String   | &check;      |
| identity   | Boolean  | &check;      |

#### ConfigurationProfile
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| displayName | String   | &check;      |
| identifier  | String   | &check;      |
| uuid        | String   | &check;      |
| version     | Int      | &check;      |

#### ExtensionAttribute
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
| value    | String   | &check;      |

#### Location
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| building     | String   | &check;      |
| department   | String   | &check;      |
| emailAddress | String   | &check;      |
| phone        | String   | &check;      |
| phoneNumber  | String   | &check;      |
| position     | String   | &check;      |
| realName     | String   | &check;      |
| realname     | String   | &check;      |
| room         | Int      | &check;      |
| username     | String   | &check;      |

#### MobileDeviceGroup
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### MobileDeviceProvisioningProfile
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| displayName       | String   | &check;      |
| expirationDate    | String   | &check;      |
| expirationDateUtc | String   | &check;      |
| uuid              | String   | &check;      |

#### Network
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| carrierSettingsVersion   | Int      | &check;      |
| cellularTechnology       | String   | &check;      |
| currentCarrierNetwork    | String   | &check;      |
| currentMobileCountryCode | Int      | &check;      |
| currentMobileNetworkCode | Int      | &check;      |
| dataRoamingEnabled       | Boolean  | &check;      |
| homeCarrierNetwork       | String   | &check;      |
| homeMobileCountryCode    | Int      | &check;      |
| homeMobileNetworkCode    | Int      | &check;      |
| iccid                    | String   | &check;      |
| imei                     | String   | &check;      |
| phoneNumber              | Long     | &check;      |
| voiceRoamingEnabled      | String   | &check;      |

#### Purchasing
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| applecareId        | String   | &check;      |
| isLeased           | Boolean  | &check;      |
| isPurchased        | Boolean  | &check;      |
| leaseExpires       | String   | &check;      |
| leaseExpiresUtc    | String   | &check;      |
| lifeExpectancy     | Int      | &check;      |
| poDate             | String   | &check;      |
| poDateUtc          | String   | &check;      |
| poNumber           | String   | &check;      |
| purchasePrice      | String   | &check;      |
| purchasingAccount  | String   | &check;      |
| purchasingContact  | String   | &check;      |
| vendor             | String   | &check;      |
| warrantyExpires    | String   | &check;      |
| warrantyExpiresUtc | String   | &check;      |

#### SecurityObject
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| activationLockEnabled           | Boolean  | &check;      |
| blockLevelEncryptionCapable     | Boolean  | &check;      |
| dataProtection                  | Boolean  | &check;      |
| fileLevelEncryptionCapable      | Boolean  | &check;      |
| hardwareEncryption              | String   | &check;      |
| jailbreakDetected               | String   | &check;      |
| lostLocationAltitude            | Double   | &check;      |
| lostLocationCourse              | Int      | &check;      |
| lostLocationHorizontalAccuracy  | Int      | &check;      |
| lostLocationLatitude            | Double   | &check;      |
| lostLocationLongitude           | Double   | &check;      |
| lostLocationSpeed               | Int      | &check;      |
| lostLocationUtc                 | String   | &check;      |
| lostLocationVerticalAccuracy    | Int      | &check;      |
| lostModeEnableIssuedUtc         | String   | &check;      |
| lostModeEnabled                 | Boolean  | &check;      |
| lostModeEnforced                | Boolean  | &check;      |
| lostModeFootnote                | String   | &check;      |
| lostModeMessage                 | String   | &check;      |
| lostModePhone                   | String   | &check;      |
| passcodeCompliant               | Boolean  | &check;      |
| passcodeCompliantWithProfile    | Boolean  | &check;      |
| passcodeLockGracePeriodEnforced | String   | &check;      |
| passcodePresent                 | Boolean  | &check;      |
