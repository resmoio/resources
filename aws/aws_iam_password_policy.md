---
description: Amazon Web Services IAM Password Policy
---
aws_iam_password_policy
-----------------------

| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| accountId                  | String   | &cross;      |
| accountName                | String   | &check;      |
| allowUsersToChangePassword | Boolean  | &check;      |
| defined                    | Boolean  | &cross;      |
| expirePasswords            | Boolean  | &check;      |
| hardExpiry                 | Boolean  | &check;      |
| maxPasswordAge             | Int      | &check;      |
| minimumPasswordLength      | Int      | &check;      |
| passwordReusePrevention    | Int      | &check;      |
| requireLowercaseCharacters | Boolean  | &check;      |
| requireNumbers             | Boolean  | &check;      |
| requireSymbols             | Boolean  | &check;      |
| requireUppercaseCharacters | Boolean  | &check;      |
