---
description: DocuSign Identity Provider
---
docusign_identity_provider
--------------------------

| **Name**             | **Type**  | **Nullable** |
| -------------------- | --------- | ------------ |
| auto_provision_users | Boolean   | &check;      |
| friendly_name        | String    | &check;      |
| id                   | String    | &cross;      |
| links                | List<Map> | &check;      |
| organizationId       | String    | &check;      |
| saml_20              | Saml20    | &check;      |
| type                 | String    | &check;      |

#### Saml20
| **Name**           | **Type**                      | **Nullable** |
| ------------------ | ----------------------------- | ------------ |
| attribute_mappings | List<Saml20.AttributeMapping> | &check;      |
| certificates       | List<Saml20.Certificate>      | &check;      |
| issuer             | String                        | &check;      |

#### Saml20.AttributeMapping
| **Name**                         | **Type** | **Nullable** |
| -------------------------------- | -------- | ------------ |
| required_attribute_friendly_name | String   | &check;      |
| required_attribute_id            | Int      | &check;      |
| required_attribute_name          | String   | &check;      |
| substitute_attribute_name        | String   | &check;      |

#### Saml20.Certificate
| **Name**        | **Type**  | **Nullable** |
| --------------- | --------- | ------------ |
| expiration_date | String    | &check;      |
| id              | String    | &check;      |
| is_valid        | Boolean   | &check;      |
| issuer          | String    | &check;      |
| links           | List<Map> | &check;      |
| thumbprint      | String    | &check;      |
