---
description: Brex Company
---
brex_company
------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| accountType    | String         | &check;      |
| id             | String         | &cross;      |
| legalName      | String         | &check;      |
| mailingAddress | MailingAddress | &check;      |

#### MailingAddress
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| city        | String   | &check;      |
| country     | String   | &check;      |
| line1       | String   | &check;      |
| line2       | String   | &check;      |
| phoneNumber | String   | &check;      |
| postalCode  | String   | &check;      |
| state       | String   | &check;      |
