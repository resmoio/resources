---
description: Azure Security Assessment
---
azure_security_assessment
-------------------------

| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| additionalData  | Map<String,String> | &check;      |
| azurePortalUri  | String             | &check;      |
| displayName     | String             | &check;      |
| id              | String             | &cross;      |
| metadata        | Metadata           | &check;      |
| name            | String             | &cross;      |
| partnersData    | PartnerData        | &check;      |
| resourceDetails | ResourceDetails    | &check;      |
| status          | AssessmentStatus   | &check;      |
| type            | String             | &cross;      |

#### AssessmentStatus
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| cause       | String   | &check;      |
| code        | String   | &check;      |
| description | String   | &check;      |

#### Metadata
| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| assessmentType         | String       | &check;      |
| categories             | List<String> | &check;      |
| description            | String       | &check;      |
| displayName            | String       | &check;      |
| implementationEffort   | String       | &check;      |
| partnerData            | PartnerData  | &check;      |
| policyDefinitionId     | String       | &check;      |
| preview                | Boolean      | &check;      |
| remediationDescription | String       | &check;      |
| severity               | String       | &check;      |
| threats                | List<String> | &check;      |
| userImpact             | String       | &check;      |

#### PartnerData
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| partnerName | String   | &check;      |
| productName | String   | &check;      |
| secret      | String   | &check;      |

#### ResourceDetails
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| id               | String   | &check;      |
| machineName      | String   | &check;      |
| sourceComputerId | String   | &check;      |
| type             | String   | &check;      |
| vmuuid           | String   | &check;      |
| workspaceId      | String   | &check;      |
