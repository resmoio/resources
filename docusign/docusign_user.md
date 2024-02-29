---
description: DocuSign User
---
docusign_user
-------------

| **Name**                     | **Type**            | **Nullable** |
| ---------------------------- | ------------------- | ------------ |
| activationAccessCode         | String              | &check;      |
| company                      | String              | &check;      |
| countryCode                  | String              | &check;      |
| createdDateTime              | String              | &check;      |
| customSettings               | List<CustomSetting> | &check;      |
| defaultAccountId             | String              | &check;      |
| email                        | String              | &check;      |
| enableConnectForUser         | String              | &check;      |
| firstName                    | String              | &check;      |
| groupList                    | List<GroupInfo>     | &check;      |
| homeAddress                  | Map<String,String>  | &check;      |
| isAdmin                      | String              | &check;      |
| jobTitle                     | String              | &check;      |
| lastLogin                    | String              | &check;      |
| lastName                     | String              | &check;      |
| loginStatus                  | String              | &check;      |
| middleName                   | String              | &check;      |
| passwordExpiration           | String              | &check;      |
| permissionProfileId          | String              | &check;      |
| permissionProfileName        | String              | &check;      |
| sendActivationEmail          | String              | &check;      |
| sendActivationOnInvalidLogin | String              | &check;      |
| subscribe                    | String              | &check;      |
| suffixName                   | String              | &check;      |
| title                        | String              | &check;      |
| uri                          | String              | &check;      |
| userId                       | String              | &cross;      |
| userName                     | String              | &check;      |
| userProfileLastModifiedDate  | String              | &check;      |
| userStatus                   | String              | &check;      |
| userType                     | String              | &check;      |
| workAddress                  | Map<String,String>  | &check;      |

#### CustomSetting
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| name          | String   | &check;      |
| originalValue | String   | &check;      |
| value         | String   | &check;      |

#### GroupInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupId  | String   | &cross;      |
