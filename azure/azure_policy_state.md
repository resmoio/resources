---
description: Azure Policy State
---
azure_policy_state
------------------

| **Name**                      | **Type**                    | **Nullable** |
| ----------------------------- | --------------------------- | ------------ |
| additionalProperties          | Map<String,JSON>            | &check;      |
| complianceState               | String                      | &check;      |
| components                    | List<ComponentStateDetails> | &check;      |
| effectiveParameters           | String                      | &check;      |
| isCompliant                   | Boolean                     | &check;      |
| managementGroupIds            | String                      | &check;      |
| policyAssignmentId            | String                      | &cross;      |
| policyAssignmentName          | String                      | &check;      |
| policyAssignmentOwner         | String                      | &check;      |
| policyAssignmentParameters    | String                      | &check;      |
| policyAssignmentScope         | String                      | &check;      |
| policyAssignmentVersion       | String                      | &check;      |
| policyDefinitionAction        | String                      | &check;      |
| policyDefinitionCategory      | String                      | &check;      |
| policyDefinitionGroupNames    | List<String>                | &check;      |
| policyDefinitionId            | String                      | &cross;      |
| policyDefinitionName          | String                      | &check;      |
| policyDefinitionReferenceId   | String                      | &check;      |
| policyDefinitionVersion       | String                      | &check;      |
| policyEvaluationDetails       | PolicyEvaluationDetails     | &check;      |
| policySetDefinitionCategory   | String                      | &check;      |
| policySetDefinitionId         | String                      | &check;      |
| policySetDefinitionName       | String                      | &check;      |
| policySetDefinitionOwner      | String                      | &check;      |
| policySetDefinitionParameters | String                      | &check;      |
| policySetDefinitionVersion    | String                      | &check;      |
| resourceGroupName             | String                      | &cross;      |
| resourceId                    | String                      | &cross;      |
| resourceLocation              | String                      | &check;      |
| resourceTags                  | String                      | &check;      |
| resourceType                  | String                      | &cross;      |
| subscriptionId                | String                      | &cross;      |

#### ComponentStateDetails
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| complianceState | String   | &check;      |
| id              | String   | &check;      |
| name            | String   | &check;      |
| timestamp       | String   | &check;      |
| type            | String   | &check;      |

#### ExpressionEvaluationDetails
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| expression      | String   | &check;      |
| expressionKind  | String   | &check;      |
| expressionValue | String   | &check;      |
| operator        | String   | &check;      |
| path            | String   | &check;      |
| result          | String   | &check;      |
| targetValue     | String   | &check;      |

#### IfNotExistsEvaluationDetails
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| resourceId     | String   | &check;      |
| totalResources | Int      | &check;      |

#### PolicyEvaluationDetails
| **Name**             | **Type**                          | **Nullable** |
| -------------------- | --------------------------------- | ------------ |
| evaluatedExpressions | List<ExpressionEvaluationDetails> | &check;      |
| ifNotExistsDetails   | IfNotExistsEvaluationDetails      | &check;      |
