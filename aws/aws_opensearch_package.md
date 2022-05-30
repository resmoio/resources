---
description: Amazon Web Services OpenSearch Package
---
aws_opensearch_package
----------------------

| **Name**                | **Type**     | **Nullable** |
| ----------------------- | ------------ | ------------ |
| accountId               | String       | &cross;      |
| availablePackageVersion | String       | &cross;      |
| createdAt               | String       | &check;      |
| description             | String       | &check;      |
| errorDetails            | ErrorDetails | &check;      |
| id                      | String       | &cross;      |
| lastUpdatedAt           | String       | &check;      |
| name                    | String       | &cross;      |
| region                  | String       | &cross;      |
| status                  | String       | &cross;      |
| type                    | String       | &cross;      |

#### ErrorDetails
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| message  | String   | &check;      |
| type     | String   | &cross;      |
