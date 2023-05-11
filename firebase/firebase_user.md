---
description: Firebase User
---
firebase_user
-------------

| **Name**             | **Type**           | **Nullable** |
| -------------------- | ------------------ | ------------ |
| creationTimestamp    | Long               | &check;      |
| customClaims         | JSON               | &check;      |
| disabled             | Boolean            | &cross;      |
| displayName          | String             | &check;      |
| email                | String             | &check;      |
| emailVerified        | Boolean            | &cross;      |
| lastRefreshTimestamp | Long               | &check;      |
| lastSignInTimestamp  | Long               | &check;      |
| phoneNumber          | String             | &check;      |
| photoUrl             | String             | &check;      |
| projectId            | String             | &cross;      |
| providers            | List<ProviderInfo> | &check;      |
| tenantId             | String             | &check;      |
| tokensValidAfter     | Long               | &check;      |
| uid                  | String             | &cross;      |

#### ProviderInfo
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &cross;      |
