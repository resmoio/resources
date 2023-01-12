---
description: Azure App Service App
---
azure_app_service_app
---------------------

| **Name**                               | **Type**                    | **Nullable** |
| -------------------------------------- | --------------------------- | ------------ |
| acrUseManagedIdentityCreds             | Boolean                     | &check;      |
| acrUserManagedIdentityId               | String                      | &check;      |
| alwaysOn                               | Boolean                     | &check;      |
| apiDefinitionUrl                       | String                      | &check;      |
| apiManagementConfigId                  | String                      | &check;      |
| appCommandLine                         | String                      | &check;      |
| appServicePlanId                       | String                      | &check;      |
| appSettings                            | Map<String,String>          | &check;      |
| authSettings                           | AuthSettings                | &check;      |
| autoHealEnabled                        | Boolean                     | &check;      |
| autoSwapSlotName                       | String                      | &check;      |
| availabilityState                      | String                      | &check;      |
| clientAffinityEnabled                  | Boolean                     | &check;      |
| clientCertEnabled                      | Boolean                     | &check;      |
| clientCertExclusionPaths               | List<String>                | &check;      |
| cloningInfo                            | CloningInfo                 | &check;      |
| connectionStrings                      | List<ConnectionString>      | &check;      |
| containerSize                          | Int                         | &check;      |
| cors                                   | CorsSettings                | &check;      |
| dailyMemoryTimeQuota                   | Int                         | &check;      |
| defaultDocuments                       | List<String>                | &check;      |
| defaultHostname                        | String                      | &check;      |
| detailedErrorLoggingEnabled            | Boolean                     | &check;      |
| documentRoot                           | String                      | &check;      |
| enabled                                | Boolean                     | &check;      |
| enabledHostNames                       | List<String>                | &check;      |
| ftpsState                              | String                      | &check;      |
| functionAppScaleLimit                  | Int                         | &check;      |
| functionsRuntimeScaleMonitoringEnabled | Boolean                     | &check;      |
| handlerMappings                        | List<HandlerMapping>        | &check;      |
| healthCheckPath                        | String                      | &check;      |
| hostNames                              | List<String>                | &check;      |
| hostingEnvironmentProfile              | HostingEnvironmentProfile   | &check;      |
| hostnameSslStates                      | List<HostnameSslState>      | &check;      |
| hostnamesDisabled                      | Boolean                     | &check;      |
| http20Enabled                          | Boolean                     | &check;      |
| httpLoggingEnabled                     | Boolean                     | &check;      |
| httpsOnly                              | Boolean                     | &check;      |
| hyperV                                 | Boolean                     | &check;      |
| id                                     | String                      | &cross;      |
| identity                               | ManagedServiceIdentity      | &check;      |
| ipSecurityRestrictions                 | List<IpSecurityRestriction> | &check;      |
| isDefaultContainer                     | Boolean                     | &check;      |
| javaContainer                          | String                      | &check;      |
| javaContainerVersion                   | String                      | &check;      |
| javaVersion                            | String                      | &check;      |
| keyVaultReferenceIdentity              | String                      | &check;      |
| lastModifiedTime                       | String                      | &check;      |
| linuxFxVersion                         | String                      | &check;      |
| loadBalancing                          | String                      | &check;      |
| localMySqlEnabled                      | Boolean                     | &check;      |
| location                               | String                      | &cross;      |
| logsDirectorySizeLimit                 | Int                         | &check;      |
| managedPipelineMode                    | String                      | &check;      |
| managedServiceIdentityId               | Int                         | &check;      |
| maxDiskSizeInMb                        | Long                        | &check;      |
| maxMemoryInMb                          | Long                        | &check;      |
| maxNumberOfWorkers                     | Int                         | &check;      |
| maxPercentageCpu                       | Double                      | &check;      |
| minTlsVersion                          | String                      | &check;      |
| minimumElasticInstanceCount            | Int                         | &check;      |
| name                                   | String                      | &cross;      |
| netFrameworkVersion                    | String                      | &check;      |
| nodeVersion                            | String                      | &check;      |
| numberOfWorkers                        | Int                         | &check;      |
| operatingSystem                        | String                      | &check;      |
| outboundIPAddresses                    | List<String>                | &check;      |
| phpVersion                             | String                      | &check;      |
| possibleOutboundIpAddresses            | List<String>                | &check;      |
| powerShellVersion                      | String                      | &check;      |
| preWarmedInstanceCount                 | Int                         | &check;      |
| publishingUsername                     | String                      | &check;      |
| push                                   | PushSettings                | &check;      |
| pythonVersion                          | String                      | &check;      |
| redundancyMode                         | String                      | &check;      |
| remoteDebuggingEnabled                 | Boolean                     | &check;      |
| remoteDebuggingVersion                 | String                      | &check;      |
| repositorySiteName                     | String                      | &check;      |
| requestTracingEnabled                  | Boolean                     | &check;      |
| requestTracingExpirationTime           | String                      | &check;      |
| resourceGroupName                      | String                      | &cross;      |
| scmIpSecurityRestrictions              | List<IpSecurityRestriction> | &check;      |
| scmIpSecurityRestrictionsUseMain       | Boolean                     | &check;      |
| scmMinTlsVersion                       | String                      | &check;      |
| scmSiteAlsoStopped                     | Boolean                     | &check;      |
| scmType                                | String                      | &check;      |
| slotSwapStatus                         | SlotSwapStatus              | &check;      |
| state                                  | String                      | &check;      |
| subscriptionId                         | String                      | &cross;      |
| suspendedTill                          | String                      | &check;      |
| tags                                   | Map<String,String>          | &check;      |
| targetSwapSlot                         | String                      | &check;      |
| tracingOptions                         | String                      | &check;      |
| trafficManagerHostNames                | List<String>                | &check;      |
| type                                   | String                      | &cross;      |
| usageState                             | String                      | &check;      |
| use32BitWorkerProcess                  | Boolean                     | &check;      |
| virtualApplications                    | List<VirtualApplication>    | &check;      |
| vnetName                               | String                      | &check;      |
| vnetPrivatePortsCount                  | Int                         | &check;      |
| vnetRouteAllEnabled                    | Boolean                     | &check;      |
| webSocketsEnabled                      | Boolean                     | &check;      |
| websiteTimeZone                        | String                      | &check;      |
| windowsFxVersion                       | String                      | &check;      |
| xManagedServiceIdentityId              | Int                         | &check;      |

#### AuthSettings
| **Name**                    | **Type**     | **Nullable** |
| --------------------------- | ------------ | ------------ |
| aadClaimsAuthorization      | String       | &check;      |
| additionalLoginParams       | List<String> | &check;      |
| allowedAudiences            | List<String> | &check;      |
| allowedExternalRedirectUrls | List<String> | &check;      |
| authFilePath                | String       | &check;      |
| clientId                    | String       | &check;      |
| configVersion               | String       | &check;      |
| defaultProvider             | String       | &check;      |
| enabled                     | Boolean      | &check;      |
| facebookAppId               | String       | &check;      |
| facebookOAuthScopes         | List<String> | &check;      |
| gitHubClientId              | String       | &check;      |
| gitHubOAuthScopes           | List<String> | &check;      |
| googleClientId              | String       | &check;      |
| googleOAuthScopes           | List<String> | &check;      |
| id                          | String       | &check;      |
| isAuthFromFile              | String       | &check;      |
| issuer                      | String       | &check;      |
| kind                        | String       | &check;      |
| microsoftAccountClientId    | String       | &check;      |
| microsoftAccountOAuthScopes | List<String> | &check;      |
| name                        | String       | &check;      |
| runtimeVersion              | String       | &check;      |
| tokenRefreshExtensionHours  | Double       | &check;      |
| tokenStoreEnabled           | Boolean      | &check;      |
| twitterConsumerKey          | String       | &check;      |
| type                        | String       | &check;      |
| unauthenticatedClientAction | String       | &check;      |
| validateIssuer              | Boolean      | &check;      |

#### CloningInfo
| **Name**                  | **Type**           | **Nullable** |
| ------------------------- | ------------------ | ------------ |
| appSettingsOverrides      | Map<String,String> | &check;      |
| cloneCustomHostNames      | Boolean            | &check;      |
| cloneSourceControl        | Boolean            | &check;      |
| configureLoadBalancing    | Boolean            | &check;      |
| correlationId             | String             | &check;      |
| hostingEnvironment        | String             | &check;      |
| overwrite                 | Boolean            | &check;      |
| sourceWebAppId            | String             | &check;      |
| sourceWebAppLocation      | String             | &check;      |
| trafficManagerProfileId   | String             | &check;      |
| trafficManagerProfileName | String             | &check;      |

#### ConnectionString
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| connectionString | String   | &check;      |
| name             | String   | &check;      |
| type             | String   | &check;      |

#### CorsSettings
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| allowedOrigins     | List<String> | &check;      |
| supportCredentials | Boolean      | &check;      |

#### HandlerMapping
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| arguments       | String   | &check;      |
| extension       | String   | &check;      |
| scriptProcessor | String   | &check;      |

#### HostingEnvironmentProfile
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### HostnameSslState
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| hostType   | String   | &check;      |
| name       | String   | &check;      |
| sslState   | String   | &check;      |
| thumbprint | String   | &check;      |
| toUpdate   | Boolean  | &check;      |
| virtualIp  | String   | &check;      |

#### IpSecurityRestriction
| **Name**             | **Type**         | **Nullable** |
| -------------------- | ---------------- | ------------ |
| action               | String           | &check;      |
| description          | String           | &check;      |
| headers              | Map<String,List> | &check;      |
| ipAddress            | String           | &check;      |
| name                 | String           | &check;      |
| priority             | Int              | &check;      |
| subnetMask           | String           | &check;      |
| subnetTrafficTag     | Int              | &check;      |
| tag                  | String           | &check;      |
| vnetSubnetResourceId | String           | &check;      |
| vnetTrafficTag       | Int              | &check;      |

#### ManagedServiceIdentity
| **Name**               | **Type**                         | **Nullable** |
| ---------------------- | -------------------------------- | ------------ |
| principalId            | String                           | &check;      |
| tenantId               | String                           | &check;      |
| type                   | String                           | &check;      |
| userAssignedIdentities | Map<String,UserAssignedIdentity> | &check;      |

#### PushSettings
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| dynamicTagsJson   | String   | &check;      |
| isPushEnabled     | Boolean  | &check;      |
| tagWhitelistJson  | String   | &check;      |
| tagsRequiringAuth | String   | &check;      |

#### SlotSwapStatus
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| destinationSlotName | String   | &check;      |
| sourceSlotName      | String   | &check;      |
| timestampUtc        | String   | &check;      |

#### UserAssignedIdentity
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| clientId    | String   | &check;      |
| principalId | String   | &check;      |

#### VirtualApplication
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| physicalPath   | String   | &check;      |
| preloadEnabled | Boolean  | &check;      |
| virtualPath    | String   | &check;      |
