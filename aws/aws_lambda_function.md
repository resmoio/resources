---
description: Amazon Web Services Lambda Function
---
aws_lambda_function
-------------------

| **Name**                 | **Type**           | **Nullable** |
| ------------------------ | ------------------ | ------------ |
| accountId                | String             | &cross;      |
| architectures            | List<String>       | &check;      |
| arn                      | String             | &cross;      |
| codeSha256               | String             | &check;      |
| codeSize                 | Long               | &check;      |
| deadLetterConfig         | DeadLetterConfig   | &check;      |
| description              | String             | &check;      |
| env                      | Map<String,String> | &cross;      |
| handler                  | String             | &check;      |
| imageConfig              | ImageConfig        | &check;      |
| kmsKeyArn                | String             | &check;      |
| layers                   | List<Layer>        | &check;      |
| masterArn                | String             | &check;      |
| memorySize               | Int                | &check;      |
| name                     | String             | &check;      |
| packageType              | String             | &check;      |
| region                   | String             | &cross;      |
| revisionId               | String             | &check;      |
| role                     | String             | &check;      |
| runtime                  | String             | &check;      |
| signingJobArn            | String             | &check;      |
| signingProfileVersionArn | String             | &check;      |
| timeout                  | Int                | &cross;      |
| tracingConfig            | TracingConfig      | &check;      |
| version                  | String             | &check;      |
| vpcConfig                | VpcConfig          | &check;      |

#### DeadLetterConfig
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| targetArn | String   | &check;      |

#### ImageConfig
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| command          | List<String> | &check;      |
| entryPoint       | List<String> | &cross;      |
| workingDirectory | String       | &check;      |

#### Layer
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| arn                      | String   | &check;      |
| signingJobArn            | String   | &check;      |
| signintProfileVersionArn | String   | &check;      |

#### TracingConfig
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| mode     | String   | &check;      |

#### VpcConfig
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| securityGroupIds | List<String> | &check;      |
| subnetIds        | List<String> | &cross;      |
| vpcId            | String       | &check;      |
