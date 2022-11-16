---
description: Google Drive Customer
---
googledrive_customer
--------------------

| **Name**       | **Type**      | **Nullable** |
| -------------- | ------------- | ------------ |
| alternateEmail | String        | &check;      |
| creationTime   | Date          | &check;      |
| domain         | String        | &check;      |
| id             | String        | &cross;      |
| language       | String        | &check;      |
| postalAddress  | PostalAddress | &check;      |

#### PostalAddress
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| addressLine1     | String   | &check;      |
| addressLine2     | String   | &check;      |
| addressLine3     | String   | &check;      |
| contactName      | String   | &check;      |
| countryCode      | String   | &check;      |
| locality         | String   | &check;      |
| organizationName | String   | &check;      |
| postalCode       | String   | &check;      |
| region           | String   | &check;      |
