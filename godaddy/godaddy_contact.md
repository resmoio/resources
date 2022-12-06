---
description: GoDaddy Contact
---
godaddy_contact
---------------

| **Name**       | **Type**       | **Nullable** |
| -------------- | -------------- | ------------ |
| _createdAt     | String         | &check;      |
| _deleted       | Boolean        | &check;      |
| _modifiedAt    | String         | &check;      |
| _revision      | Int            | &check;      |
| addressMailing | AddressMailing | &check;      |
| domainId       | String         | &check;      |
| email          | String         | &cross;      |
| encoding       | String         | &check;      |
| exposeWhois    | Boolean        | &check;      |
| fax            | String         | &check;      |
| jobTitle       | String         | &check;      |
| nameFirst      | String         | &check;      |
| nameLast       | String         | &check;      |
| nameMiddle     | String         | &check;      |
| organization   | String         | &check;      |
| phone          | String         | &check;      |
| tlds           | List<String>   | &check;      |
| type           | String         | &check;      |

#### AddressMailing
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| address1   | String   | &check;      |
| address2   | String   | &check;      |
| city       | String   | &check;      |
| country    | String   | &check;      |
| postalCode | String   | &check;      |
| state      | String   | &check;      |
