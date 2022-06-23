---
description: Jamf Pro Computer
---
jamf_computer
-------------

| **Name**                   | **Type**                   | **Nullable** |
| -------------------------- | -------------------------- | ------------ |
| altMacAddress              | String                     | &check;      |
| altNetworkAdapterType      | String                     | &check;      |
| assetTag                   | String                     | &check;      |
| barcode1                   | String                     | &check;      |
| barcode2                   | String                     | &check;      |
| certificates               | List<Certificate>          | &check;      |
| configurationProfiles      | List<ConfigurationProfile> | &check;      |
| distributionPoint          | String                     | &check;      |
| extensionAttributes        | List<ExtensionAttribute>   | &check;      |
| groupsAccounts             | GroupsAccounts             | &check;      |
| hardware                   | Hardware                   | &check;      |
| id                         | Int                        | &cross;      |
| initialEntryDate           | String                     | &check;      |
| initialEntryDateUtc        | String                     | &check;      |
| ipAddress                  | String                     | &check;      |
| itunesStoreAccountIsActive | Boolean                    | &check;      |
| jamfVersion                | String                     | &check;      |
| lastCloudBackupDateUtc     | String                     | &check;      |
| lastContactTime            | String                     | &check;      |
| lastContactTimeUtc         | String                     | &check;      |
| lastEnrolledDateUtc        | String                     | &check;      |
| lastReportedIp             | String                     | &check;      |
| location                   | Location                   | &check;      |
| macAddress                 | String                     | &check;      |
| managementStatus           | ManagementStatus           | &check;      |
| mdmCapable                 | Boolean                    | &check;      |
| mdmCapableUsers            | MdmCapableUsers            | &check;      |
| name                       | String                     | &check;      |
| networkAdapterType         | String                     | &check;      |
| peripherals                | List<Peripheral>           | &check;      |
| platform                   | String                     | &check;      |
| purchasing                 | Purchasing                 | &check;      |
| remoteManagement           | RemoteManagement           | &check;      |
| reportDate                 | String                     | &check;      |
| reportDateUtc              | String                     | &check;      |
| security                   | Security                   | &check;      |
| serialNumber               | String                     | &check;      |
| serverName                 | String                     | &cross;      |
| site                       | Site                       | &check;      |
| software                   | Software                   | &check;      |
| sus                        | String                     | &check;      |
| udid                       | String                     | &check;      |

#### Application
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| path     | String   | &check;      |
| version  | String   | &check;      |

#### Attachment
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| filename | String   | &check;      |
| id       | Int      | &check;      |
| uri      | String   | &check;      |

#### AvailableUpdate
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| name        | String   | &check;      |
| packageName | String   | &check;      |
| version     | String   | &check;      |

#### Certificate
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| commonName | String   | &check;      |
| expires    | Long     | &check;      |
| expiresUtc | String   | &check;      |
| identify   | Boolean  | &check;      |
| name       | String   | &check;      |

#### ConfigurationProfile
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| id          | Int      | &check;      |
| isRemovable | Boolean  | &check;      |
| name        | String   | &check;      |
| uuid        | String   | &check;      |

#### ExtensionAttribute
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
| value    | Int      | &check;      |

#### Filevault2User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| user     | String   | &check;      |

#### Font
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| path     | String   | &check;      |
| version  | String   | &check;      |

#### GroupsAccounts
| **Name**                 | **Type**           | **Nullable** |
| ------------------------ | ------------------ | ------------ |
| computerGroupMemberships | List<String>       | &check;      |
| localAccounts            | List<LocalAccount> | &check;      |

#### Hardware
| **Name**                    | **Type**             | **Nullable** |
| --------------------------- | -------------------- | ------------ |
| activeDirectoryStatus       | String               | &check;      |
| availableRamSlots           | Int                  | &check;      |
| batteryCapacity             | Int                  | &check;      |
| bleCapable                  | Boolean              | &check;      |
| bootRom                     | String               | &check;      |
| busSpeed                    | Int                  | &check;      |
| busSpeedMhz                 | Int                  | &check;      |
| cacheSize                   | Int                  | &check;      |
| cacheSizeKb                 | Int                  | &check;      |
| diskEncryptionConfiguration | String               | &check;      |
| filevault2Users             | List<Filevault2User> | &check;      |
| gatekeeperStatus            | String               | &check;      |
| institutionalRecoveryKey    | String               | &check;      |
| make                        | String               | &check;      |
| mappedPrinters              | List<MappedPrinter>  | &check;      |
| masterPasswordSet           | Boolean              | &check;      |
| model                       | String               | &check;      |
| modelIdentifier             | String               | &check;      |
| nicSpeed                    | String               | &check;      |
| numberCores                 | Int                  | &check;      |
| numberProcessors            | Int                  | &check;      |
| opticalDrive                | String               | &check;      |
| osBuild                     | String               | &check;      |
| osName                      | String               | &check;      |
| osVersion                   | String               | &check;      |
| processorArchitechture      | String               | &check;      |
| processorSpeed              | Int                  | &check;      |
| processorSpeedMhz           | Int                  | &check;      |
| processorType               | String               | &check;      |
| servicePack                 | String               | &check;      |
| sipStatus                   | String               | &check;      |
| smcVersion                  | String               | &check;      |
| storage                     | List<Storage>        | &check;      |
| totalRam                    | Int                  | &check;      |
| totalRamMb                  | Int                  | &check;      |
| xprotectVersion             | Int                  | &check;      |

#### LocalAccount
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| administrator    | Boolean  | &check;      |
| filevaultEnabled | Boolean  | &check;      |
| home             | String   | &check;      |
| homeSize         | String   | &check;      |
| homeSizeMb       | Int      | &check;      |
| name             | String   | &check;      |
| realname         | String   | &check;      |
| uid              | Int      | &check;      |

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

#### ManagementStatus
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| enrolledViaDep         | Boolean  | &check;      |
| userApprovedEnrollment | Boolean  | &check;      |
| userApprovedMdm        | Boolean  | &check;      |

#### MappedPrinter
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| location | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |
| uri      | String   | &check;      |

#### MdmCapableUsers
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| mdmCapableUser | String   | &check;      |

#### Partition
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| bootDriveAvailableMb | Int      | &check;      |
| filevault2Percent    | Int      | &check;      |
| filevault2Status     | String   | &check;      |
| filevaultPercent     | Int      | &check;      |
| filevaultStatus      | String   | &check;      |
| lvUUID               | String   | &check;      |
| lvgUUID              | String   | &check;      |
| name                 | String   | &check;      |
| partitionCapacityMb  | Int      | &check;      |
| pvUUID               | String   | &check;      |
| size                 | Int      | &check;      |
| type                 | String   | &check;      |

#### Peripheral
| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| attachments | List<Attachment> | &check;      |
| peripheral  | JSON             | &check;      |
| purchasing  | Purchasing       | &check;      |

#### Plugin
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| path     | String   | &check;      |
| version  | String   | &check;      |

#### Purchasing
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| applecareId          | String   | &check;      |
| isLeased             | Boolean  | &check;      |
| isPurchased          | Boolean  | &check;      |
| leaseExpires         | String   | &check;      |
| leaseExpiresUtc      | String   | &check;      |
| lifeExpectancy       | Int      | &check;      |
| poDate               | String   | &check;      |
| poDateUtc            | String   | &check;      |
| poNumber             | String   | &check;      |
| purchasePrice        | String   | &check;      |
| purchasingAccount    | String   | &check;      |
| purchasingContact    | String   | &check;      |
| vendor               | String   | &check;      |
| warrantyExpires      | String   | &check;      |
| warrantyExpiresEpoch | Int      | &check;      |
| warrantyExpiresUtc   | String   | &check;      |

#### RemoteManagement
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| managed            | Boolean  | &check;      |
| managementUsername | String   | &check;      |

#### Security
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| activationLock      | Boolean  | &check;      |
| externalBootLevel   | String   | &check;      |
| firewallEnabled     | Boolean  | &check;      |
| recoveryLockEnabled | Boolean  | &check;      |
| secureBootLevel     | String   | &check;      |

#### Site
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | Int      | &check;      |
| name     | String   | &check;      |

#### Software
| **Name**                 | **Type**              | **Nullable** |
| ------------------------ | --------------------- | ------------ |
| applications             | List<Application>     | &check;      |
| availableSoftwareUpdates | List<String>          | &check;      |
| availableUpdates         | List<AvailableUpdate> | &check;      |
| cachedByCasper           | List<String>          | &check;      |
| fonts                    | List<Font>            | &check;      |
| installedByCasper        | List<String>          | &check;      |
| installedByInstallerSwu  | List<String>          | &check;      |
| licensedSoftware         | List<String>          | &check;      |
| plugins                  | List<Plugin>          | &check;      |
| runningServices          | List<String>          | &check;      |
| unixExecutables          | List<String>          | &check;      |

#### Storage
| **Name**        | **Type**        | **Nullable** |
| --------------- | --------------- | ------------ |
| connectionType  | String          | &check;      |
| disk            | String          | &check;      |
| driveCapacityMb | Int             | &check;      |
| model           | String          | &check;      |
| partition       | List<Partition> | &check;      |
| revision        | String          | &check;      |
| serialNumber    | String          | &check;      |
| size            | Int             | &check;      |
| smartStatus     | String          | &check;      |
