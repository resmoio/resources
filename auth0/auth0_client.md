---
description: Auth0 Client
---
auth0_client
------------

| **Name**                      | **Type**              | **Nullable** |
| ----------------------------- | --------------------- | ------------ |
| addons                        | Addons                | &check;      |
| allowed_clients               | List<String>          | &check;      |
| allowed_logout_urls           | List<String>          | &check;      |
| allowed_origins               | List<String>          | &check;      |
| app_type                      | String                | &check;      |
| callbacks                     | List<String>          | &check;      |
| client_aliases                | List<String>          | &check;      |
| client_id                     | String                | &cross;      |
| cross_origin_loc              | String                | &check;      |
| custom_login_page             | String                | &check;      |
| custom_login_page_on          | Boolean               | &check;      |
| custom_login_page_preview     | String                | &check;      |
| description                   | String                | &check;      |
| encryption_key                | EncryptionKey         | &check;      |
| form_template                 | String                | &check;      |
| global                        | Boolean               | &check;      |
| grant_types                   | List<String>          | &check;      |
| initiate_login_uri            | String                | &check;      |
| is_first_party                | Boolean               | &check;      |
| jwt_configuration             | JwtConfiguration      | &check;      |
| logo_uri                      | String                | &check;      |
| mobile                        | Mobile                | &check;      |
| name                          | String                | &check;      |
| native_social_login           | NativeSocialLogin     | &check;      |
| oidc_backchannel_logout       | OidcBackchannelLogout | &check;      |
| oidc_conformant               | Boolean               | &check;      |
| organization_require_behavior | String                | &check;      |
| organization_usage            | String                | &check;      |
| refresh_token                 | RefreshToken          | &check;      |
| sso                           | Boolean               | &check;      |
| sso_disabled                  | Boolean               | &check;      |
| tenant                        | String                | &check;      |
| token_endpoint_auth_method    | String                | &check;      |
| web_origins                   | List<String>          | &check;      |

#### Addons
| **Name**               | **Type**                    | **Nullable** |
| ---------------------- | --------------------------- | ------------ |
| aws                    | Addons.Aws                  | &check;      |
| azure_blob             | Addons.AzureBlob            | &check;      |
| azure_sb               | Addons.AzureSb              | &check;      |
| echosign               | Addons.Echosign             | &check;      |
| egnyte                 | Addons.Egnyte               | &check;      |
| firebase               | Addons.Firebase             | &check;      |
| layer                  | Addons.Layer                | &check;      |
| mscrm                  | Addons.Mscrm                | &check;      |
| newrelic               | Addons.Newrelic             | &check;      |
| office365              | Addons.Office365            | &check;      |
| rms                    | Addons.Rms                  | &check;      |
| salesforce             | Addons.Salesforce           | &check;      |
| salesforce_api         | Addons.SalesforceApi        | &check;      |
| salesforce_sandbox_api | Addons.SalesforceSandboxApi | &check;      |
| samlp                  | Addons.Samlp                | &check;      |
| sap_api                | Addons.SapApi               | &check;      |
| sentry                 | Addons.Sentry               | &check;      |
| sharepoint             | Addons.Sharepoint           | &check;      |
| slack                  | Addons.Slack                | &check;      |
| springcm               | Addons.Springcm             | &check;      |
| sso_integration        | Addons.SsoIntegration       | &check;      |
| wams                   | Addons.Wams                 | &check;      |
| zendesk                | Addons.Zendesk              | &check;      |
| zoom                   | Addons.Zoom                 | &check;      |

#### Addons.Aws
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| lifetime_in_seconds | Int      | &check;      |
| principal           | String   | &check;      |
| role                | String   | &check;      |

#### Addons.AzureBlob
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| accountName      | String   | &check;      |
| blobName         | String   | &check;      |
| blob_delete      | Boolean  | &check;      |
| blob_read        | Boolean  | &check;      |
| blob_write       | Boolean  | &check;      |
| containerName    | String   | &check;      |
| container_delete | Boolean  | &check;      |
| container_list   | Boolean  | &check;      |
| container_read   | Boolean  | &check;      |
| container_write  | Boolean  | &check;      |
| expiration       | Int      | &check;      |
| signedIdentifier | String   | &check;      |
| storageAccessKey | String   | &check;      |

#### Addons.AzureSb
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| entityPath | String   | &check;      |
| expiration | Int      | &check;      |
| namespace  | String   | &check;      |
| sasKey     | String   | &check;      |
| sasKeyName | String   | &check;      |

#### Addons.Echosign
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &check;      |

#### Addons.Egnyte
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &check;      |

#### Addons.Firebase
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| client_email        | String   | &check;      |
| lifetime_in_seconds | Int      | &check;      |
| private_key_id      | String   | &check;      |

#### Addons.Layer
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| expiration | Int      | &check;      |
| keyId      | String   | &check;      |
| principal  | String   | &check;      |
| privateKey | String   | &check;      |
| providerId | String   | &check;      |

#### Addons.Mscrm
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| url      | String   | &check;      |

#### Addons.Newrelic
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| account  | String   | &check;      |

#### Addons.Office365
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| connection | String   | &check;      |
| domain     | String   | &check;      |

#### Addons.Rms
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| url      | String   | &check;      |

#### Addons.Salesforce
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| entity_id | String   | &check;      |

#### Addons.SalesforceApi
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| clientid              | String   | &check;      |
| communityName         | String   | &check;      |
| community_url_section | String   | &check;      |
| principal             | String   | &check;      |

#### Addons.SalesforceSandboxApi
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| clientid              | String   | &check;      |
| communityName         | String   | &check;      |
| community_url_section | String   | &check;      |
| principal             | String   | &check;      |

#### Addons.Samlp
| **Name**                       | **Type**     | **Nullable** |
| ------------------------------ | ------------ | ------------ |
| audience                       | String       | &check;      |
| authnContextClassRef           | String       | &check;      |
| createUpnClaim                 | Boolean      | &check;      |
| destination                    | String       | &check;      |
| digestAlgorithm                | String       | &check;      |
| issuer                         | String       | &check;      |
| lifetimeInSeconds              | Int          | &check;      |
| mapIdentities                  | Boolean      | &check;      |
| mapUnknownClaimsAsIs           | Boolean      | &check;      |
| nameIdentifierFormat           | String       | &check;      |
| nameIdentifierProbes           | List<String> | &check;      |
| passthroughClaimsWithNoMapping | Boolean      | &check;      |
| recipient                      | String       | &check;      |
| signResponse                   | Boolean      | &check;      |
| signatureAlgorithm             | String       | &check;      |

#### Addons.SapApi
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| clientid             | String   | &check;      |
| nameIdentifierFormat | String   | &check;      |
| scope                | String   | &check;      |
| servicePassword      | String   | &check;      |
| tokenEndpointUrl     | String   | &check;      |
| usernameAttribute    | String   | &check;      |

#### Addons.Sentry
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| base_url | String   | &check;      |
| org_slug | String   | &check;      |

#### Addons.Sharepoint
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| external_url | List<String> | &check;      |
| url          | String       | &check;      |

#### Addons.Slack
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| team     | String   | &check;      |

#### Addons.Springcm
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| acsurl   | String   | &check;      |

#### Addons.SsoIntegration
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| version  | String   | &check;      |

#### Addons.Wams
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| masterkey | String   | &check;      |

#### Addons.Zendesk
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| accountName | String   | &check;      |

#### Addons.Zoom
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| account  | String   | &check;      |

#### EncryptionKey
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| cert     | String   | &check;      |
| pub      | String   | &check;      |
| subject  | String   | &check;      |

#### JwtConfiguration
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| alg                 | String   | &check;      |
| lifetime_in_seconds | Int      | &check;      |
| secret_encoded      | Boolean  | &check;      |

#### Mobile
| **Name** | **Type**       | **Nullable** |
| -------- | -------------- | ------------ |
| android  | Mobile.Android | &check;      |
| ios      | Mobile.Ios     | &check;      |

#### Mobile.Android
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| app_package_name | String   | &check;      |

#### Mobile.Ios
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| app_bundle_identifier | String   | &check;      |
| team_id               | String   | &check;      |

#### NativeSocialLogin
| **Name** | **Type**                   | **Nullable** |
| -------- | -------------------------- | ------------ |
| apple    | NativeSocialLogin.Apple    | &check;      |
| facebook | NativeSocialLogin.Facebook | &check;      |

#### NativeSocialLogin.Apple
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### NativeSocialLogin.Facebook
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |

#### OidcBackchannelLogout
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| backchannel_logout_urls | List<String> | &check;      |

#### RefreshToken
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| expiration_type              | String   | &check;      |
| idle_token_lifetime          | Int      | &check;      |
| infinite_idle_token_lifetime | Boolean  | &check;      |
| infinite_token_lifetime      | Boolean  | &check;      |
| leeway                       | Int      | &check;      |
| rotation_type                | String   | &check;      |
| token_lifetime               | Int      | &check;      |
