---
description: Amazon Web Services IAM Identity Center Group
---
aws_iam_identity_center_group
-----------------------------

| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| accountId       | String       | &cross;      |
| displayName     | String       | &cross;      |
| groupId         | String       | &cross;      |
| identityStoreId | String       | &cross;      |
| memberships     | List<Member> | &cross;      |
| region          | String       | &cross;      |

#### Member
| **Name**     | **Type**        | **Nullable** |
| ------------ | --------------- | ------------ |
| memberId     | Member.MemberId | &check;      |
| membershipId | String          | &cross;      |

#### Member.MemberId
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
| type     | String   | &cross;      |
