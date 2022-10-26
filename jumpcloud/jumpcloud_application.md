---
description: JumpCloud Application
---
jumpcloud_application
---------------------

| **Name**           | **Type**         | **Nullable** |
| ------------------ | ---------------- | ------------ |
| active             | Boolean          | &check;      |
| beta               | Boolean          | &check;      |
| color              | String           | &check;      |
| config             | Config           | &check;      |
| created            | String           | &check;      |
| databaseAttributes | List<Attributes> | &check;      |
| description        | String           | &check;      |
| displayLabel       | String           | &check;      |
| displayName        | String           | &check;      |
| id                 | String           | &cross;      |
| learnMore          | String           | &check;      |
| logo               | Logo             | &check;      |
| logoFile           | LogoFile         | &check;      |
| name               | String           | &check;      |
| organizationId     | String           | &cross;      |
| organizationName   | String           | &cross;      |
| sso                | Sso              | &check;      |
| ssoUrl             | String           | &check;      |
| userGroups         | List<String>     | &cross;      |

#### Attributes
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| dependsOnProperty | String   | &check;      |
| label             | String   | &check;      |
| mutable           | Boolean  | &check;      |
| options           | String   | &check;      |
| position          | Int      | &check;      |
| readOnly          | Boolean  | &check;      |
| required          | Boolean  | &check;      |
| toggle            | String   | &check;      |
| type              | String   | &check;      |
| value             | String   | &check;      |
| valueType         | String   | &check;      |
| visible           | Boolean  | &check;      |

#### Config
| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| acsUrl                  | Attributes              | &check;      |
| constantAttributes      | ListOfValueAttributes   | &check;      |
| databaseAttributes      | ListOfValueAttributes   | &check;      |
| declareRedirectEndpoint | Attributes              | &check;      |
| defaultTargetUrl        | Attributes              | &check;      |
| groupsAttributeName     | Attributes              | &check;      |
| idpCertificate          | Attributes              | &check;      |
| idpEntityId             | Attributes              | &check;      |
| idpInitUrl              | Attributes              | &check;      |
| idpPrivateKey           | Attributes              | &check;      |
| includeGroups           | Attributes              | &check;      |
| overrideNameIdFormat    | ListOfOptionsAttributes | &check;      |
| signAssertion           | Attributes              | &check;      |
| signatureAlgorithm      | ListOfOptionsAttributes | &check;      |
| spCertificate           | Attributes              | &check;      |
| spEntityId              | Attributes              | &check;      |
| subjectField            | ListOfOptionsAttributes | &check;      |

#### ListOfOptionsAttributes
| **Name**          | **Type**     | **Nullable** |
| ----------------- | ------------ | ------------ |
| dependsOnProperty | String       | &check;      |
| label             | String       | &check;      |
| mutable           | Boolean      | &check;      |
| options           | List<Option> | &check;      |
| position          | Int          | &check;      |
| readOnly          | Boolean      | &check;      |
| required          | Boolean      | &check;      |
| toggle            | String       | &check;      |
| type              | String       | &check;      |
| value             | String       | &check;      |
| visible           | Boolean      | &check;      |

#### ListOfValueAttributes
| **Name**          | **Type**    | **Nullable** |
| ----------------- | ----------- | ------------ |
| dependsOnProperty | String      | &check;      |
| label             | String      | &check;      |
| mutable           | Boolean     | &check;      |
| options           | String      | &check;      |
| position          | Int         | &check;      |
| readOnly          | Boolean     | &check;      |
| required          | Boolean     | &check;      |
| toggle            | String      | &check;      |
| type              | String      | &check;      |
| value             | List<Value> | &check;      |
| visible           | Boolean     | &check;      |

#### Logo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| url      | String   | &check;      |

#### LogoFile
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| contentType | String   | &check;      |
| fileName    | String   | &check;      |
| fileSize    | Int      | &check;      |
| id          | String   | &check;      |
| storage     | String   | &check;      |

#### Option
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| text     | String   | &check;      |
| value    | Int      | &check;      |

#### Sso
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| beta                | Boolean  | &check;      |
| idpCertExpirationAt | String   | &check;      |
| jit                 | Boolean  | &check;      |
| type                | String   | &check;      |

#### Value
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| readOnly | Boolean  | &check;      |
| required | Boolean  | &check;      |
| value    | String   | &check;      |
| visible  | Boolean  | &check;      |
