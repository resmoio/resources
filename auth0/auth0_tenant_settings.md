---
description: Auth0 Tenant Settings
---
auth0_tenant_settings
---------------------

| **Name**                   | **Type**        | **Nullable** |
| -------------------------- | --------------- | ------------ |
| allowed_logout_urls        | List<String>    | &check;      |
| change_password            | ChangePassword  | &check;      |
| default_audience           | String          | &check;      |
| default_directory          | String          | &check;      |
| default_redirection_uri    | String          | &check;      |
| device_flow                | DeviceFlow      | &check;      |
| enabled_locales            | List<String>    | &check;      |
| error_page                 | ErrorPage       | &check;      |
| flags                      | Flags           | &check;      |
| friendly_name              | String          | &check;      |
| guardian_mfa_page          | GuardianMfaPage | &check;      |
| idle_session_lifetime      | Int             | &check;      |
| sandbox_version            | String          | &check;      |
| sandbox_versions_available | List<String>    | &check;      |
| session_cookie             | SessionCookie   | &check;      |
| session_lifetime           | Int             | &check;      |
| support_email              | String          | &check;      |
| support_url                | String          | &check;      |

#### ChangePassword
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |
| html     | String   | &check;      |

#### DeviceFlow
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| charset  | String   | &check;      |
| mask     | String   | &check;      |

#### ErrorPage
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| html          | String   | &check;      |
| show_log_link | Boolean  | &check;      |
| url           | String   | &check;      |

#### Flags
| **Name**                                            | **Type** | **Nullable** |
| --------------------------------------------------- | -------- | ------------ |
| allow_changing_enable_sso                           | Boolean  | &check;      |
| allow_legacy_delegation_grant_types                 | Boolean  | &check;      |
| allow_legacy_ro_grant_types                         | Boolean  | &check;      |
| allow_legacy_tokeninfo_endpoint                     | Boolean  | &check;      |
| change_pwd_flow_v1                                  | Boolean  | &check;      |
| dashboard_insights_view                             | Boolean  | &check;      |
| dashboard_log_streams_next                          | Boolean  | &check;      |
| disable_clickjack_protection_headers                | Boolean  | &check;      |
| disable_fields_map_fix                              | Boolean  | &check;      |
| disable_impersonation                               | Boolean  | &check;      |
| enable_adfs_waad_email_verification                 | Boolean  | &check;      |
| enable_apis_section                                 | Boolean  | &check;      |
| enable_client_connections                           | Boolean  | &check;      |
| enable_idtoken_api2                                 | Boolean  | &check;      |
| enable_legacy_profile                               | Boolean  | &check;      |
| enable_pipeline2                                    | Boolean  | &check;      |
| enable_public_signup_user_exists_error              | Boolean  | &check;      |
| enable_sso                                          | Boolean  | &check;      |
| enforce_client_authentication_on_passwordless_start | Boolean  | &check;      |
| no_disclose_enterprise_connections                  | Boolean  | &check;      |
| revoke_refresh_token_grant                          | Boolean  | &check;      |

#### GuardianMfaPage
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| enabled  | Boolean  | &check;      |
| html     | String   | &check;      |

#### SessionCookie
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| mode     | String   | &check;      |
