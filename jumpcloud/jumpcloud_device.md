---
description: JumpCloud Device
---
jumpcloud_device
----------------

| **Name**                       | **Type**               | **Nullable** |
| ------------------------------ | ---------------------- | ------------ |
| active                         | Boolean                | &check;      |
| agentVersion                   | String                 | &check;      |
| allowMultiFactorAuthentication | Boolean                | &check;      |
| allowPublicKeyAuthentication   | Boolean                | &check;      |
| allowSshPasswordAuthentication | Boolean                | &check;      |
| allowSshRootLogin              | Boolean                | &check;      |
| amazonInstanceID               | String                 | &check;      |
| arch                           | String                 | &check;      |
| azureAdJoined                  | Boolean                | &check;      |
| builtInCommands                | List<BuiltInCommand>   | &check;      |
| connectionHistory              | List<Map>              | &check;      |
| created                        | String                 | &check;      |
| description                    | String                 | &check;      |
| deviceGroups                   | List<String>           | &cross;      |
| displayManager                 | String                 | &check;      |
| displayName                    | String                 | &check;      |
| domainInfo                     | DomainInfo             | &check;      |
| fde                            | Fde                    | &check;      |
| fileSystem                     | String                 | &check;      |
| hasServiceAccount              | Boolean                | &check;      |
| hostname                       | String                 | &check;      |
| id                             | String                 | &cross;      |
| lastContact                    | String                 | &check;      |
| mdm                            | Mdm                    | &check;      |
| modifySSHDConfig               | Boolean                | &check;      |
| networkInterfaces              | List<NetworkInterface> | &check;      |
| organization                   | String                 | &check;      |
| organizationId                 | String                 | &cross;      |
| organizationName               | String                 | &cross;      |
| os                             | String                 | &check;      |
| osFamily                       | String                 | &check;      |
| osVersionDetail                | OsVersionDetail        | &check;      |
| provisionMetadata              | ProvisionMetadata      | &check;      |
| remoteIP                       | String                 | &check;      |
| serialNumber                   | String                 | &check;      |
| serviceAccountState            | ServiceAccountState    | &check;      |
| sshRootEnabled                 | Boolean                | &check;      |
| sshdParams                     | List<SshdParam>        | &check;      |
| systemInsights                 | SystemInsights         | &check;      |
| systemTimezone                 | Int                    | &check;      |
| tags                           | List<String>           | &check;      |
| templateName                   | String                 | &check;      |
| userMetrics                    | List<UserMetric>       | &check;      |
| version                        | String                 | &check;      |

#### BuiltInCommand
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| type     | String   | &check;      |

#### DomainInfo
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| domainName   | String   | &check;      |
| partOfDomain | Boolean  | &check;      |

#### Fde
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| active     | Boolean  | &check;      |
| keyPresent | Boolean  | &check;      |

#### Mdm
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| dep               | Boolean  | &check;      |
| deviceId          | String   | &check;      |
| enrollmentType    | String   | &check;      |
| profileIdentifier | String   | &check;      |
| userApproved      | Boolean  | &check;      |
| vendor            | String   | &check;      |

#### NetworkInterface
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| address  | String   | &check;      |
| family   | String   | &check;      |
| internal | Boolean  | &check;      |
| name     | String   | &check;      |

#### OsVersionDetail
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| major       | String   | &check;      |
| minor       | String   | &check;      |
| osName      | String   | &check;      |
| patch       | String   | &check;      |
| releaseName | String   | &check;      |
| revision    | String   | &check;      |

#### ProvisionMetadata
| **Name**    | **Type**    | **Nullable** |
| ----------- | ----------- | ------------ |
| provisioner | Provisioner | &check;      |

#### Provisioner
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| provisionerId | String   | &check;      |
| type          | String   | &check;      |

#### ServiceAccountState
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| hasSecureToken    | Boolean  | &check;      |
| passwordAPFSValid | Boolean  | &check;      |
| passwordODValid   | Boolean  | &check;      |

#### SshdParam
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### SystemInsights
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| state    | String   | &check;      |

#### User
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| email    | String   | &cross;      |
| name     | String   | &cross;      |

#### UserMetric
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| admin              | Boolean  | &check;      |
| managed            | Boolean  | &check;      |
| secureTokenEnabled | Boolean  | &check;      |
| suspended          | Boolean  | &check;      |
| userName           | String   | &check;      |
