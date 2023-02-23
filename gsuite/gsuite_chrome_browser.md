---
description: Google Workspace Chrome Browser
---
gsuite_chrome_browser
---------------------

| **Name**                 | **Type**                 | **Nullable** |
| ------------------------ | ------------------------ | ------------ |
| annotatedAssetId         | String                   | &check;      |
| browserVersions          | List<String>             | &check;      |
| browsers                 | List<Browser>            | &check;      |
| deviceId                 | String                   | &cross;      |
| deviceIdentifiersHistory | DeviceIdentifiersHistory | &check;      |
| extensionCount           | String                   | &check;      |
| lastActivityTime         | String                   | &check;      |
| lastDeviceUser           | String                   | &check;      |
| lastDeviceUsers          | List<LastDeviceUser>     | &check;      |
| lastPolicyFetchTime      | String                   | &check;      |
| lastRegistrationTime     | String                   | &check;      |
| lastStatusReportTime     | String                   | &check;      |
| machineName              | String                   | &check;      |
| machinePolicies          | List<MachinePolicy>      | &check;      |
| orgUnitPath              | String                   | &check;      |
| osArchitecture           | String                   | &check;      |
| osPlatform               | String                   | &check;      |
| osPlatformVersion        | String                   | &check;      |
| osVersion                | String                   | &check;      |
| policyCount              | String                   | &check;      |
| virtualDeviceId          | String                   | &check;      |

#### Browser
| **Name**             | **Type**      | **Nullable** |
| -------------------- | ------------- | ------------ |
| browserVersion       | String        | &check;      |
| channel              | String        | &check;      |
| executablePath       | String        | &check;      |
| lastStatusReportTime | String        | &check;      |
| plugins              | List<Plugin>  | &check;      |
| profiles             | List<Profile> | &check;      |

#### DeviceIdentifiersHistory
| **Name** | **Type**                              | **Nullable** |
| -------- | ------------------------------------- | ------------ |
| records  | List<DeviceIdentifiersHistory.Record> | &check;      |

#### DeviceIdentifiersHistory.Record
| **Name**         | **Type**                                    | **Nullable** |
| ---------------- | ------------------------------------------- | ------------ |
| firstRecordTime  | String                                      | &check;      |
| identifiers      | DeviceIdentifiersHistory.Record.Identifiers | &check;      |
| lastActivityTime | String                                      | &check;      |

#### DeviceIdentifiersHistory.Record.Identifiers
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| machineName | String   | &check;      |

#### Extension
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| appType         | String       | &check;      |
| description     | String       | &check;      |
| disabled        | Boolean      | &check;      |
| extensionId     | String       | &cross;      |
| homepageUrl     | String       | &check;      |
| installType     | String       | &check;      |
| manifestVersion | Int          | &check;      |
| name            | String       | &check;      |
| permissions     | List<String> | &check;      |
| version         | String       | &check;      |

#### LastDeviceUser
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| lastStatusReportTime | String   | &check;      |
| userName             | String   | &check;      |

#### MachinePolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| source   | String   | &check;      |
| value    | String   | &check;      |

#### Plugin
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| description | String   | &check;      |
| filename    | String   | &check;      |
| name        | String   | &check;      |

#### Profile
| **Name**                | **Type**        | **Nullable** |
| ----------------------- | --------------- | ------------ |
| chromeSignedInUserEmail | String          | &check;      |
| extensions              | List<Extension> | &check;      |
| id                      | String          | &cross;      |
| lastPolicyFetchTime     | String          | &check;      |
| lastStatusReportTime    | String          | &check;      |
| name                    | String          | &check;      |
