---
description: Salesforce User
---
salesforce_user
---------------

| **Name**               | **Type**   | **Nullable** |
| ---------------------- | ---------- | ------------ |
| address                | Address    | &check;      |
| alias                  | String     | &check;      |
| attributes             | Attributes | &check;      |
| communityNickname      | String     | &check;      |
| companyName            | String     | &check;      |
| createdById            | String     | &check;      |
| createdDate            | String     | &check;      |
| department             | String     | &check;      |
| details                | JSON       | &check;      |
| division               | String     | &check;      |
| email                  | String     | &check;      |
| fax                    | String     | &check;      |
| firstName              | String     | &check;      |
| id                     | String     | &cross;      |
| isActive               | Boolean    | &check;      |
| lastLoginDate          | String     | &check;      |
| lastModifiedById       | String     | &check;      |
| lastModifiedDate       | String     | &check;      |
| lastName               | String     | &check;      |
| lastPasswordChangeDate | String     | &check;      |
| managerId              | String     | &check;      |
| mobilePhone            | String     | &check;      |
| name                   | String     | &check;      |
| numberOfFailedLogins   | Int        | &check;      |
| phone                  | String     | &check;      |
| profileId              | String     | &check;      |
| systemModstamp         | String     | &check;      |
| title                  | String     | &check;      |
| userRoleId             | String     | &check;      |
| userType               | String     | &check;      |
| username               | String     | &check;      |

#### Address
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| city            | String   | &check;      |
| country         | String   | &check;      |
| geocodeAccuracy | String   | &check;      |
| latitude        | Double   | &check;      |
| longitude       | Double   | &check;      |
| postalCode      | String   | &check;      |
| state           | String   | &check;      |
| stateCode       | String   | &check;      |
| street          | String   | &check;      |

#### Attributes
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| type     | String   | &check;      |
| url      | String   | &check;      |
