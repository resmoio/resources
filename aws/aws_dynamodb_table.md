---
description: Amazon Web Services DynamoDB Table
---
aws_dynamodb_table
------------------

| **Name**           | **Type**                     | **Nullable** |
| ------------------ | ---------------------------- | ------------ |
| accountId          | String                       | &cross;      |
| arn                | String                       | &cross;      |
| attributes         | List<Attribute>              | &cross;      |
| backup             | ContinuousBackupsDescription | &cross;      |
| billingMode        | String                       | &check;      |
| capacity           | Capacity                     | &check;      |
| classSummary       | ClassSummary                 | &check;      |
| creationDate       | String                       | &cross;      |
| encryption         | Encryption                   | &check;      |
| globalTableVersion | String                       | &check;      |
| gsi                | List<GSI>                    | &cross;      |
| keySchema          | List<KeySchema>              | &cross;      |
| name               | String                       | &cross;      |
| region             | String                       | &cross;      |
| replicas           | List<Replica>                | &check;      |
| status             | String                       | &cross;      |
| streamType         | String                       | &check;      |

#### Attribute
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &cross;      |
| type     | String   | &cross;      |

#### Capacity
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| lastDecreaseTime    | String   | &check;      |
| lastIncreaseTime    | String   | &check;      |
| numOfDecreasesToday | Long     | &cross;      |
| read                | Long     | &cross;      |
| write               | Long     | &cross;      |

#### ClassSummary
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| class    | String   | &cross;      |

#### ContinuousBackupsDescription
| **Name**                  | **Type** | **Nullable** |
| ------------------------- | -------- | ------------ |
| pointInTimeRecoveryStatus | String   | &check;      |
| status                    | String   | &check;      |

#### Encryption
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| kmsMasterKeyArn | String   | &check;      |
| status          | String   | &cross;      |
| type            | String   | &cross;      |

#### GSI
| **Name**   | **Type**        | **Nullable** |
| ---------- | --------------- | ------------ |
| capacity   | Capacity        | &check;      |
| keySchema  | List<KeySchema> | &cross;      |
| name       | String          | &cross;      |
| projection | String          | &cross;      |
| status     | String          | &cross;      |

#### KeySchema
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| attributeName | String   | &cross;      |
| type          | String   | &cross;      |

#### Replica
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| region   | String   | &cross;      |
| status   | String   | &cross;      |
