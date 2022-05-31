---
description: Amazon Web Services IAM Credential Report
---
aws_iam_credential_report
-------------------------

| **Name**                | **Type**   | **Nullable** |
| ----------------------- | ---------- | ------------ |
| accessKey1Active        | String     | &check;      |
| accessKey1LastRotatedIn | LastUsedIn | &cross;      |
| accessKey1LastUsedIn    | LastUsedIn | &cross;      |
| accessKey2Active        | String     | &check;      |
| accessKey2LastRotatedIn | LastUsedIn | &cross;      |
| accessKey2LastUsedIn    | LastUsedIn | &cross;      |
| accountId               | String     | &cross;      |
| arn                     | String     | &cross;      |
| cert1Active             | String     | &check;      |
| cert1LastRotatedIn      | LastUsedIn | &cross;      |
| cert2Active             | String     | &check;      |
| cert2LastRotatedIn      | LastUsedIn | &cross;      |
| generatedTime           | String     | &cross;      |
| mfaActive               | String     | &check;      |
| passwordEnabled         | String     | &check;      |
| passwordLastUsedIn      | LastUsedIn | &cross;      |
| passwordNextRotation    | String     | &check;      |
| user                    | String     | &cross;      |
| userCreationTime        | String     | &check;      |

#### LastUsedIn
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| fortyFiveDays | Boolean  | &cross;      |
| oneMonth      | Boolean  | &cross;      |
| oneWeek       | Boolean  | &cross;      |
| threeMonths   | Boolean  | &cross;      |
| twoMonths     | Boolean  | &cross;      |
