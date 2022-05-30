---
description: Azure Virtual Machine
---
azure_virtual_machine
---------------------

| **Name**                                        | **Type**                        | **Nullable** |
| ----------------------------------------------- | ------------------------------- | ------------ |
| applicationProfile                              | ApplicationProfile              | &check;      |
| availabilitySetId                               | String                          | &check;      |
| availabilityZones                               | Set                             | &check;      |
| billingProfile                                  | BillingProfile                  | &check;      |
| bootDiagnosticsStorageUri                       | String                          | &check;      |
| capacityReservationGroupId                      | String                          | &check;      |
| computerName                                    | String                          | &check;      |
| dataDisks                                       | Map<Int,VirtualMachineDataDisk> | &check;      |
| diagnosticsProfile                              | DiagnosticsProfile              | &check;      |
| evictionPolicy                                  | String                          | &check;      |
| extensions                                      | List<VirtualMachineExtension>   | &check;      |
| extensionsTimeBudget                            | String                          | &check;      |
| hardwareProfile                                 | HardwareProfile                 | &check;      |
| hostGroupId                                     | String                          | &check;      |
| hostId                                          | String                          | &check;      |
| id                                              | String                          | &cross;      |
| instanceView                                    | VirtualMachineInstanceView      | &check;      |
| isBootDiagnosticsEnabled                        | Boolean                         | &check;      |
| isHibernationEnabled                            | Boolean                         | &check;      |
| isManagedDiskEnabled                            | Boolean                         | &check;      |
| isManagedServiceIdentityEnabled                 | Boolean                         | &check;      |
| isOSDiskEphemeral                               | Boolean                         | &check;      |
| isUltraSsdEnabled                               | Boolean                         | &check;      |
| licenseType                                     | String                          | &check;      |
| managedServiceIdentityType                      | String                          | &check;      |
| name                                            | String                          | &cross;      |
| networkProfile                                  | NetworkProfile                  | &check;      |
| osDiskCachingType                               | String                          | &check;      |
| osDiskDeleteOptions                             | String                          | &check;      |
| osDiskDiskEncryptionSetId                       | String                          | &check;      |
| osDiskId                                        | String                          | &check;      |
| osDiskSize                                      | Int                             | &check;      |
| osDiskStorageAccountType                        | String                          | &check;      |
| osProfile                                       | OSProfile                       | &check;      |
| osType                                          | String                          | &check;      |
| osUnmanagedDiskVhdUri                           | String                          | &check;      |
| plan                                            | Plan                            | &check;      |
| platformFaultDomain                             | Int                             | &check;      |
| powerState                                      | String                          | &check;      |
| primaryPublicIPAddress                          | PublicIpAddress                 | &check;      |
| primaryPublicIPAddressId                        | String                          | &check;      |
| priority                                        | String                          | &check;      |
| provisioningState                               | String                          | &check;      |
| proximityPlacementGroup                         | ProximityPlacementGroup         | &check;      |
| resourceGroupName                               | String                          | &cross;      |
| securityProfile                                 | SecurityProfile                 | &check;      |
| size                                            | String                          | &check;      |
| storageProfile                                  | StorageProfile                  | &check;      |
| subscriptionId                                  | String                          | &cross;      |
| systemAssignedManagedServiceIdentityPrincipalId | String                          | &check;      |
| systemAssignedManagedServiceIdentityTenantId    | String                          | &check;      |
| tags                                            | Map<String,String>              | &check;      |
| terminateNotificationProfile                    | TerminateNotificationProfile    | &check;      |
| type                                            | String                          | &cross;      |
| unmanagedDataDisks                              | Map<Int,VirtualMachineDataDisk> | &check;      |
| userAssignedManagedServiceIdentityIds           | Set                             | &check;      |
| userData                                        | String                          | &check;      |

#### AdditionalUnattendContent
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| componentName | String   | &check;      |
| content       | String   | &check;      |
| passName      | String   | &check;      |
| settingName   | String   | &check;      |

#### ApplicationProfile
| **Name**            | **Type**                 | **Nullable** |
| ------------------- | ------------------------ | ------------ |
| galleryApplications | List<GalleryApplication> | &check;      |

#### BillingProfile
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| maxPrice | Double   | &check;      |

#### BootDiagnostics
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| enabled    | Boolean  | &check;      |
| storageUri | String   | &check;      |

#### BootDiagnosticsInstanceView
| **Name**                 | **Type**           | **Nullable** |
| ------------------------ | ------------------ | ------------ |
| consoleScreenshotBlobUri | String             | &check;      |
| serialConsoleLogBlobUri  | String             | &check;      |
| status                   | InstanceViewStatus | &check;      |

#### DataDisk
| **Name**                | **Type**              | **Nullable** |
| ----------------------- | --------------------- | ------------ |
| caching                 | String                | &check;      |
| createOption            | String                | &check;      |
| detachOption            | String                | &check;      |
| diskDeleteOption        | String                | &check;      |
| diskIopsReadWrite       | Long                  | &check;      |
| diskMBpsReadWrite       | Long                  | &check;      |
| diskSizeGB              | Int                   | &check;      |
| imageUri                | String                | &check;      |
| lun                     | Int                   | &check;      |
| managedDisk             | ManagedDiskParameters | &check;      |
| name                    | String                | &check;      |
| toBeDetached            | Boolean               | &check;      |
| vhdUri                  | String                | &check;      |
| writeAcceleratorEnabled | Boolean               | &check;      |

#### DiagnosticsProfile
| **Name**        | **Type**        | **Nullable** |
| --------------- | --------------- | ------------ |
| bootDiagnostics | BootDiagnostics | &cross;      |

#### DiskDiffSettings
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| option    | String   | &check;      |
| placement | String   | &check;      |

#### DiskEncryptionSettings
| **Name**          | **Type**                | **Nullable** |
| ----------------- | ----------------------- | ------------ |
| diskEncryptionKey | KeyVaultSecretReference | &check;      |
| enabled           | Boolean                 | &check;      |
| keyEncryptionKey  | KeyVaultSecretReference | &check;      |

#### DiskInstanceView
| **Name**           | **Type**                     | **Nullable** |
| ------------------ | ---------------------------- | ------------ |
| encryptionSettings | List<DiskEncryptionSettings> | &check;      |
| name               | String                       | &check;      |
| statuses           | List<InstanceViewStatus>     | &check;      |

#### GalleryApplication
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| configurationReference | String   | &check;      |
| order                  | Int      | &check;      |
| packageReferenceId     | String   | &check;      |
| tags                   | String   | &check;      |

#### HardwareProfile
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| vCpusAvailable | Int      | &check;      |
| vCpusPerCore   | Int      | &check;      |
| vmSize         | String   | &check;      |

#### ImageReference
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| communityGalleryImageId | String   | &check;      |
| offer                   | String   | &check;      |
| publisher               | String   | &check;      |
| sharedGalleryImageId    | String   | &check;      |
| sku                     | String   | &check;      |
| version                 | String   | &check;      |

#### InstanceViewStatus
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| code          | String   | &check;      |
| displayStatus | String   | &check;      |
| level         | String   | &check;      |
| message       | String   | &check;      |

#### KeyVaultSecretReference
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| secretUrl   | String   | &check;      |
| sourceVault | JSON     | &check;      |

#### LinuxConfiguration
| **Name**                      | **Type**           | **Nullable** |
| ----------------------------- | ------------------ | ------------ |
| disablePasswordAuthentication | Boolean            | &check;      |
| patchSettings                 | LinuxPatchSettings | &check;      |
| provisionVMAgent              | Boolean            | &check;      |
| publicKeys                    | List<SshPublicKey> | &check;      |

#### LinuxPatchSettings
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| assessmentMode | String   | &check;      |
| patchMode      | String   | &check;      |

#### MaintenanceRedeployStatus
| **Name**                              | **Type** | **Nullable** |
| ------------------------------------- | -------- | ------------ |
| isCustomerInitiatedMaintenanceAllowed | Boolean  | &check;      |
| lastOperationResultCode               | String   | &check;      |
| maintenanceWindowEndTime              | String   | &check;      |
| maintenanceWindowStartTime            | String   | &check;      |
| preMaintenanceWindowEndTime           | String   | &check;      |
| preMaintenanceWindowStartTime         | String   | &check;      |

#### ManagedDiskParameters
| **Name**              | **Type**              | **Nullable** |
| --------------------- | --------------------- | ------------ |
| diskEncryptionSet     | String                | &check;      |
| storageAccountType    | String                | &check;      |
| vmDiskSecurityProfile | VMDiskSecurityProfile | &check;      |

#### NetworkInterfaceReference
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| deleteOption | String   | &check;      |
| id           | String   | &check;      |
| primary      | Boolean  | &check;      |

#### NetworkProfile
| **Name**          | **Type**                        | **Nullable** |
| ----------------- | ------------------------------- | ------------ |
| networkApiVersion | String                          | &check;      |
| networkInterfaces | List<NetworkInterfaceReference> | &check;      |

#### OSDisk
| **Name**                | **Type**               | **Nullable** |
| ----------------------- | ---------------------- | ------------ |
| caching                 | String                 | &check;      |
| deleteOption            | String                 | &check;      |
| diskDiffSettings        | DiskDiffSettings       | &check;      |
| diskSizeGB              | Int                    | &check;      |
| encryptionSettings      | DiskEncryptionSettings | &check;      |
| imageUri                | String                 | &check;      |
| managedDisk             | ManagedDiskParameters  | &check;      |
| name                    | String                 | &check;      |
| osType                  | String                 | &check;      |
| vhdUri                  | String                 | &check;      |
| writeAcceleratorEnabled | Boolean                | &check;      |

#### OSProfile
| **Name**                    | **Type**               | **Nullable** |
| --------------------------- | ---------------------- | ------------ |
| adminPassword               | String                 | &check;      |
| adminUsername               | String                 | &check;      |
| allowExtensionOperations    | Boolean                | &check;      |
| computerName                | String                 | &check;      |
| customData                  | String                 | &check;      |
| linuxConfiguration          | LinuxConfiguration     | &check;      |
| requireGuestProvisionSignal | Boolean                | &check;      |
| secrets                     | List<VaultSecretGroup> | &check;      |
| windowsConfiguration        | WindowsConfiguration   | &check;      |

#### PatchSettings
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| assessmentMode    | String   | &check;      |
| enableHotpatching | Boolean  | &check;      |
| patchMode         | String   | &check;      |

#### Plan
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| name          | String   | &check;      |
| product       | String   | &check;      |
| promotionCode | String   | &check;      |
| publisher     | String   | &check;      |

#### ProximityPlacementGroup
| **Name**                    | **Type**     | **Nullable** |
| --------------------------- | ------------ | ------------ |
| availabilitySetIds          | List<String> | &check;      |
| id                          | String       | &cross;      |
| location                    | String       | &check;      |
| proximityPlacementGroupType | String       | &check;      |
| resourceGroupName           | String       | &check;      |
| virtualMachineIds           | List<String> | &check;      |
| virtualMachineScaleSetIds   | List<String> | &check;      |

#### PublicIpAddress
| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| assignedLoadBalancerFrontend | JSON         | &check;      |
| availabilityZones            | List<String> | &check;      |
| fqdn                         | String       | &check;      |
| hasAssignedLoadBalancer      | Boolean      | &check;      |
| hasAssignedNetworkInterface  | Boolean      | &cross;      |
| idleTimeoutInMinutes         | Int          | &check;      |
| ipAddress                    | String       | &check;      |
| ipAllocationMethod           | String       | &check;      |
| ipTags                       | List<String> | &check;      |
| leafDomainLabel              | String       | &check;      |
| nicIpConfiguration           | JSON         | &check;      |
| reverseFqdn                  | String       | &check;      |
| sku                          | String       | &check;      |
| version                      | String       | &check;      |

#### SecurityProfile
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| encryptionAtHostEnabled | Boolean      | &check;      |
| securityType            | String       | &check;      |
| uefiSettings            | UefiSettings | &check;      |

#### SshPublicKey
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| keyData  | String   | &check;      |
| path     | String   | &check;      |

#### StorageProfile
| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| dataDisks      | List<DataDisk> | &check;      |
| imageReference | ImageReference | &check;      |
| osDisk         | OSDisk         | &check;      |

#### TerminateNotificationProfile
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| enable           | Boolean  | &check;      |
| notBeforeTimeout | String   | &check;      |

#### UefiSettings
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| secureBootEnabled | Boolean  | &check;      |
| vTpmEnabled       | Boolean  | &check;      |

#### VMDiskSecurityProfile
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| diskEncryptionSet      | String   | &check;      |
| securityEncryptionType | String   | &check;      |

#### VaultCertificate
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| certificateStore | String   | &check;      |
| certificateUrl   | String   | &check;      |

#### VaultSecretGroup
| **Name**          | **Type**               | **Nullable** |
| ----------------- | ---------------------- | ------------ |
| sourceVault       | JSON                   | &check;      |
| vaultCertificates | List<VaultCertificate> | &check;      |

#### VirtualMachineAgentInstanceView
| **Name**          | **Type**                                  | **Nullable** |
| ----------------- | ----------------------------------------- | ------------ |
| extensionHandlers | List<VirtualMachineExtensionInstanceView> | &check;      |
| statuses          | List<InstanceViewStatus>                  | &check;      |
| vmAgentVersion    | String                                    | &check;      |

#### VirtualMachineDataDisk
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| cachingType         | String   | &check;      |
| creationMethod      | String   | &check;      |
| deleteOptions       | String   | &check;      |
| diskEncryptionSetId | String   | &check;      |
| lun                 | Int      | &check;      |
| size                | Int      | &check;      |
| sourceImageUri      | String   | &check;      |
| storageAccountType  | String   | &check;      |
| vhdUri              | String   | &check;      |

#### VirtualMachineExtension
| **Name**                       | **Type**           | **Nullable** |
| ------------------------------ | ------------------ | ------------ |
| autoUpgradeMinorVersionEnabled | Boolean            | &check;      |
| forceUpdateTag                 | String             | &check;      |
| id                             | String             | &check;      |
| location                       | String             | &check;      |
| name                           | String             | &check;      |
| provisioningState              | String             | &check;      |
| publicSettings                 | JSON               | &check;      |
| publisher                      | String             | &check;      |
| suppressFailures               | Boolean            | &check;      |
| tags                           | Map<String,String> | &check;      |
| type                           | String             | &check;      |
| typeHandlerVersion             | String             | &check;      |
| version                        | String             | &check;      |

#### VirtualMachineExtensionInstanceView
| **Name**           | **Type**                 | **Nullable** |
| ------------------ | ------------------------ | ------------ |
| name               | String                   | &check;      |
| statuses           | List<InstanceViewStatus> | &check;      |
| substatuses        | List<InstanceViewStatus> | &check;      |
| type               | String                   | &check;      |
| typeHandlerVersion | String                   | &check;      |

#### VirtualMachineInstanceView
| **Name**                  | **Type**                                  | **Nullable** |
| ------------------------- | ----------------------------------------- | ------------ |
| assignedHost              | String                                    | &check;      |
| bootDiagnostics           | BootDiagnosticsInstanceView               | &check;      |
| computerName              | String                                    | &check;      |
| disks                     | List<DiskInstanceView>                    | &check;      |
| extensions                | List<VirtualMachineExtensionInstanceView> | &check;      |
| hyperVGeneration          | String                                    | &check;      |
| maintenanceRedeployStatus | MaintenanceRedeployStatus                 | &check;      |
| osName                    | String                                    | &check;      |
| osVersion                 | String                                    | &check;      |
| platformFaultDomain       | Int                                       | &check;      |
| platformUpdateDomain      | Int                                       | &check;      |
| rdpThumbPrint             | String                                    | &check;      |
| statuses                  | List<InstanceViewStatus>                  | &check;      |
| vmAgent                   | VirtualMachineAgentInstanceView           | &check;      |
| vmHealth                  | InstanceViewStatus                        | &check;      |

#### WinRMConfiguration
| **Name**  | **Type**            | **Nullable** |
| --------- | ------------------- | ------------ |
| listeners | List<WinRMListener> | &check;      |

#### WinRMListener
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| certificateUrl | String   | &check;      |
| protocol       | String   | &check;      |

#### WindowsConfiguration
| **Name**                  | **Type**                        | **Nullable** |
| ------------------------- | ------------------------------- | ------------ |
| additionalUnattendContent | List<AdditionalUnattendContent> | &check;      |
| enableAutomaticUpdates    | Boolean                         | &check;      |
| patchSettings             | PatchSettings                   | &check;      |
| provisionVMAgent          | Boolean                         | &check;      |
| timeZone                  | String                          | &check;      |
| winRM                     | WinRMConfiguration              | &check;      |
