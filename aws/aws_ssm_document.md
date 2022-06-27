---
description: Amazon Web Services SSM Document
---
aws_ssm_document
----------------

| **Name**        | **Type**               | **Nullable** |
| --------------- | ---------------------- | ------------ |
| accountId       | String                 | &cross;      |
| author          | String                 | &check;      |
| createdDate     | String                 | &check;      |
| displayName     | String                 | &check;      |
| documentFormat  | String                 | &check;      |
| documentType    | String                 | &check;      |
| documentVersion | String                 | &check;      |
| name            | String                 | &cross;      |
| owner           | String                 | &check;      |
| platformTypes   | List<String>           | &check;      |
| region          | String                 | &cross;      |
| requires        | List<DocumentRequires> | &check;      |
| reviewStatus    | String                 | &check;      |
| schemaVersion   | String                 | &check;      |
| tags            | Map<String,String>     | &check;      |
| targetType      | String                 | &check;      |
| versionName     | String                 | &check;      |

#### DocumentRequires
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| version  | String   | &check;      |
