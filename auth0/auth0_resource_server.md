---
description: Auth0 Resource Server
---
auth0_resource_server
---------------------

| **Name**                                        | **Type**  | **Nullable** |
| ----------------------------------------------- | --------- | ------------ |
| allow_offline_access                            | Boolean   | &check;      |
| enforce_policies                                | Boolean   | &check;      |
| id                                              | String    | &cross;      |
| identifier                                      | String    | &check;      |
| is_system                                       | Boolean   | &check;      |
| name                                            | String    | &check;      |
| scopes                                          | List<Map> | &check;      |
| signing_alg                                     | String    | &check;      |
| skip_consent_for_verifiable_first_party_clients | Boolean   | &check;      |
| token_dialect                                   | String    | &check;      |
| token_lifetime                                  | Int       | &check;      |
| token_lifetime_for_web                          | Int       | &check;      |
