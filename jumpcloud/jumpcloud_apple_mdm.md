---
description: JumpCloud Apple MDM
---
jumpcloud_apple_mdm
-------------------

| **Name**                              | **Type** | **Nullable** |
| ------------------------------------- | -------- | ------------ |
| ades                                  | Ades     | &check;      |
| allowMobileUserEnrollment             | Boolean  | &check;      |
| apnsCertExpiry                        | String   | &check;      |
| apnsPushTopic                         | String   | &check;      |
| defaultIosUserEnrollmentDeviceGroupID | String   | &check;      |
| defaultSystemGroupID                  | String   | &check;      |
| dep                                   | Dep      | &check;      |
| depAccessTokenExpiry                  | String   | &check;      |
| depServerTokenState                   | String   | &check;      |
| id                                    | String   | &cross;      |
| name                                  | String   | &check;      |
| organizationId                        | String   | &cross;      |
| organizationName                      | String   | &cross;      |

#### Ades
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| ios      | Ios      | &check;      |
| macos    | Macos    | &check;      |

#### Dep
| **Name**                  | **Type**                   | **Nullable** |
| ------------------------- | -------------------------- | ------------ |
| enableZeroTouchEnrollment | Boolean                    | &check;      |
| setupAssistantOptions     | List<SetupAssistantOption> | &check;      |
| welcomeScreen             | WelcomeScreen              | &check;      |

#### Ios
| **Name**                    | **Type**                   | **Nullable** |
| --------------------------- | -------------------------- | ------------ |
| defaultDeviceGroupObjectIds | List<String>               | &check;      |
| enableZeroTouchEnrollment   | Boolean                    | &check;      |
| setupAssistantOptions       | List<SetupAssistantOption> | &check;      |
| welcomeScreen               | WelcomeScreen              | &check;      |

#### Macos
| **Name**                    | **Type**                   | **Nullable** |
| --------------------------- | -------------------------- | ------------ |
| defaultDeviceGroupObjectIds | List<String>               | &check;      |
| enableZeroTouchEnrollment   | Boolean                    | &check;      |
| setupAssistantOptions       | List<SetupAssistantOption> | &check;      |
| welcomeScreen               | WelcomeScreen              | &check;      |

#### SetupAssistantOption
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| option   | String   | &check;      |

#### WelcomeScreen
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| button    | String   | &check;      |
| paragraph | String   | &check;      |
| title     | String   | &check;      |
