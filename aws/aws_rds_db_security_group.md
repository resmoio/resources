---
description: Amazon Web Services RDS DB Security Group
---
aws_rds_db_security_group
-------------------------

| **Name**          | **Type**               | **Nullable** |
| ----------------- | ---------------------- | ------------ |
| accountId         | String                 | &cross;      |
| arn               | String                 | &cross;      |
| description       | String                 | &check;      |
| ec2SecurityGroups | List<EC2SecurityGroup> | &check;      |
| ipRanges          | List<IPRange>          | &check;      |
| name              | String                 | &cross;      |
| ownerId           | String                 | &cross;      |
| region            | String                 | &cross;      |
| vpcId             | String                 | &check;      |

#### EC2SecurityGroup
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| ec2SecurityGroupId      | String   | &cross;      |
| ec2SecurityGroupName    | String   | &check;      |
| ec2SecurityGroupOwnerId | String   | &cross;      |
| status                  | String   | &check;      |

#### IPRange
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| cidrip   | String   | &check;      |
| status   | String   | &check;      |

#### ResourceCustomComparable
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |

