---
description: Amazon Web Services Glue Catalog Database
---
aws_glue_catalog_database
-------------------------

| **Name**                      | **Type**                  | **Nullable** |
| ----------------------------- | ------------------------- | ------------ |
| accountId                     | String                    | &cross;      |
| catalogId                     | String                    | &check;      |
| createTableDefaultPermissions | List<PrincipalPermission> | &check;      |
| createTime                    | String                    | &check;      |
| description                   | String                    | &check;      |
| locationUri                   | String                    | &check;      |
| name                          | String                    | &cross;      |
| parameters                    | Map<String,String>        | &check;      |
| region                        | String                    | &cross;      |
| targetDatabase                | DatabaseIdentifier        | &check;      |

#### DataLakePrincipal
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| dataLakePrincipalIdentifier | String   | &check;      |

#### DatabaseIdentifier
| **Name**     | **Type** | **Nullable** |
| ------------ | -------- | ------------ |
| catalogId    | String   | &check;      |
| databaseName | String   | &check;      |

#### PrincipalPermission
| **Name**    | **Type**          | **Nullable** |
| ----------- | ----------------- | ------------ |
| permissions | List<String>      | &check;      |
| principal   | DataLakePrincipal | &check;      |
