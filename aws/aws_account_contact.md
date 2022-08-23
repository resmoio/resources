---
description: Amazon Web Services Account Contact
---
aws_account_contact
-------------------

| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| accountId   | String           | &cross;      |
| accountName | String           | &check;      |
| billing     | AlternateContact | &check;      |
| operations  | AlternateContact | &check;      |
| primary     | Contact          | &check;      |
| security    | AlternateContact | &check;      |

#### AlternateContact
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| emailAddress | String   | &cross;      |
| name         | String   | &cross;      |
| phoneNumber  | String   | &cross;      |
| title        | String   | &cross;      |

#### Contact
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| addressLine1     | String   | &check;      |
| addressLine2     | String   | &check;      |
| addressLine3     | String   | &check;      |
| city             | String   | &check;      |
| companyName      | String   | &check;      |
| countryCode      | String   | &check;      |
| districtOrCounty | String   | &check;      |
| fullName         | String   | &check;      |
| phoneNumber      | String   | &check;      |
| postalCode       | String   | &check;      |
| stateOrRegion    | String   | &check;      |
| websiteUrl       | String   | &check;      |
