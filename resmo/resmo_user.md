---
description: Resmo User
---
resmo_user
----------

| **Name**    | **Type**             | **Nullable** |
| ----------- | -------------------- | ------------ |
| accountId   | String               | &cross;      |
| createdAt   | Timestamp            | &cross;      |
| email       | String               | &cross;      |
| id          | String               | &cross;      |
| isEnabled   | Boolean              | &cross;      |
| isVerified  | Boolean              | &cross;      |
| memberships | List<MembershipInfo> | &check;      |
| mfaEnabled  | Boolean              | &check;      |
| name        | String               | &cross;      |

#### MembershipInfo
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| isOwner          | Boolean  | &cross;      |
| membershipActive | Boolean  | &cross;      |
| product          | String   | &cross;      |
| role             | String   | &cross;      |
