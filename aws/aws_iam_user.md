---
description: Amazon Web Services IAM User
---
aws_iam_user
------------

| **Name**            | **Type**             | **Nullable** |
| ------------------- | -------------------- | ------------ |
| accessKeys          | List<AccessKey>      | &cross;      |
| accountId           | String               | &cross;      |
| accountName         | String               | &check;      |
| arn                 | String               | &cross;      |
| attachedPolicies    | List<AttachedPolicy> | &cross;      |
| createdDate         | String               | &cross;      |
| groups              | List<Group>          | &cross;      |
| mfaDevices          | List<MFADevice>      | &cross;      |
| passwordLastUsed    | String               | &check;      |
| passwordLastUsedIn  | PasswordLastUsed     | &check;      |
| permissionsBoundary | PermissionsBoundary  | &check;      |
| policies            | List<Policy>         | &cross;      |
| userId              | String               | &cross;      |
| username            | String               | &cross;      |

#### AccessKey
| **Name**    | **Type**           | **Nullable** |
| ----------- | ------------------ | ------------ |
| createdDate | String             | &cross;      |
| id          | String             | &cross;      |
| lastUsedIn  | AccessKey.LastUsed | &check;      |
| status      | String             | &cross;      |

#### AccessKey.LastUsed
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| fortyFiveDays | Boolean  | &cross;      |
| oneMonth      | Boolean  | &cross;      |
| oneWeek       | Boolean  | &cross;      |
| threeMonths   | Boolean  | &cross;      |
| twoMonths     | Boolean  | &cross;      |

#### AttachedPolicy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &cross;      |
| name     | String   | &cross;      |

#### Group
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| arn        | String   | &cross;      |
| createDate | String   | &check;      |
| groupId    | String   | &cross;      |
| groupName  | String   | &cross;      |
| path       | String   | &check;      |

#### MFADevice
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| enableDate   | String   | &cross;      |
| serialNumber | String   | &cross;      |

#### PasswordLastUsed
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| fortyFiveDays | Boolean  | &cross;      |
| oneMonth      | Boolean  | &cross;      |
| oneWeek       | Boolean  | &cross;      |
| threeMonths   | Boolean  | &cross;      |
| twoMonths     | Boolean  | &cross;      |

#### PermissionsBoundary
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &cross;      |
| type     | String   | &cross;      |

#### Policy
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| document | JSON     | &check;      |
| name     | String   | &cross;      |
