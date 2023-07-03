---
description: Amazon Web Services Lambda Layer
---
aws_lambda_layer
----------------

| **Name**              | **Type**     | **Nullable** |
| --------------------- | ------------ | ------------ |
| accountId             | String       | &cross;      |
| accountName           | String       | &check;      |
| arn                   | String       | &cross;      |
| latestMatchingVersion | LayerVersion | &check;      |
| name                  | String       | &check;      |
| region                | String       | &cross;      |

#### LayerVersion
| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| compatibleArchitectures | List<String> | &check;      |
| compatibleRuntimes      | List<String> | &check;      |
| createdDate             | String       | &check;      |
| description             | String       | &check;      |
| layerVersionArn         | String       | &cross;      |
| licenseInfo             | String       | &check;      |
| version                 | Long         | &check;      |
