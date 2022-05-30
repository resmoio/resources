---
description: Amazon Web Services Account Contact
---
aws_account_contact
-------------------

| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| accountId  | String   | &cross;      |
| billing    | Contact  | &check;      |
| operations | Contact  | &check;      |
| security   | Contact  | &check;      |

#### Contact
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| emailAddress | String   | &cross;      |
| name         | String   | &cross;      |
| phoneNumber  | String   | &cross;      |
| title        | String   | &cross;      |
