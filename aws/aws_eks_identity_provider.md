---
description: Amazon Web Services EKS Identity Provider
---
aws_eks_identity_provider
-------------------------

| **Name**       | **Type**           | **Nullable** |
| -------------- | ------------------ | ------------ |
| accountId      | String             | &cross;      |
| accountName    | String             | &check;      |
| arn            | String             | &cross;      |
| clientId       | String             | &check;      |
| clusterName    | String             | &check;      |
| groupsClaim    | String             | &check;      |
| groupsPrefix   | String             | &check;      |
| issuerUrl      | String             | &check;      |
| name           | String             | &cross;      |
| region         | String             | &cross;      |
| requiredClaims | Map<String,String> | &check;      |
| status         | String             | &check;      |
| tags           | Map<String,String> | &check;      |
| usernameClaim  | String             | &check;      |
| usernamePrefix | String             | &check;      |
