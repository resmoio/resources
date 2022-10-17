---
description: Qualys Web App Scan
---
qualys_web_app_scan
-------------------

| **Name**   | **Type**   | **Nullable** |
| ---------- | ---------- | ------------ |
| id         | String     | &cross;      |
| launchDate | String     | &check;      |
| launchedBy | LaunchedBy | &check;      |
| mode       | String     | &check;      |
| multi      | Boolean    | &check;      |
| name       | String     | &check;      |
| profile    | Profile    | &check;      |
| reference  | String     | &check;      |
| status     | String     | &check;      |
| summary    | Summary    | &check;      |
| target     | TargetInfo | &check;      |
| type       | String     | &check;      |

#### LaunchedBy
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| firstName | String   | &check;      |
| id        | String   | &check;      |
| lastName  | String   | &check;      |
| username  | String   | &check;      |

#### Profile
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |

#### Summary
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| authStatus    | String   | &check;      |
| crawlDuration | String   | &check;      |
| linksCrawled  | String   | &check;      |
| nbRequests    | String   | &check;      |
| resultsStatus | String   | &check;      |
| testDuration  | String   | &check;      |

#### TargetInfo
| **Name**         | **Type**                    | **Nullable** |
| ---------------- | --------------------------- | ------------ |
| cancelOption     | String                      | &check;      |
| scannerAppliance | TargetInfo.ScannerAppliance | &check;      |
| webApp           | TargetInfo.WebApp           | &check;      |

#### TargetInfo.ScannerAppliance
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |

#### TargetInfo.WebApp
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |
| name     | String   | &check;      |
| url      | String   | &check;      |
