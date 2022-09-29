---
description: Google Cloud Platform GCP Organization
---
gcp_organization
----------------

| **Name**       | **Type**      | **Nullable** |
| -------------- | ------------- | ------------ |
| contacts       | List<Contact> | &check;      |
| creationTime   | String        | &check;      |
| displayName    | String        | &check;      |
| lifecycleState | String        | &check;      |
| name           | String        | &cross;      |
| owner          | Owner         | &check;      |

#### Contact
| **Name**                          | **Type**     | **Nullable** |
| --------------------------------- | ------------ | ------------ |
| email                             | String       | &check;      |
| languageTag                       | String       | &check;      |
| name                              | String       | &check;      |
| notificationCategorySubscriptions | List<String> | &check;      |
| validateTime                      | String       | &check;      |
| validationState                   | String       | &check;      |

#### GCPResource
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| groupKey | String   | &cross;      |

#### Owner
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| directoryCustomerId | String   | &cross;      |
