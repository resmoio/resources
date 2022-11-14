---
description: Amazon Web Services Network Firewall Policy
---
aws_networkfirewall_policy
--------------------------

| **Name**                        | **Type**                          | **Nullable** |
| ------------------------------- | --------------------------------- | ------------ |
| accountId                       | String                            | &cross;      |
| accountName                     | String                            | &check;      |
| arn                             | String                            | &cross;      |
| name                            | String                            | &check;      |
| region                          | String                            | &cross;      |
| statefulDefaultActions          | List<String>                      | &check;      |
| statefulEngineOptions           | StatefulEngineOptions             | &check;      |
| statefulRuleGroupReferences     | List<StatefulRuleGroupReference>  | &check;      |
| statelessCustomActions          | List<CustomAction>                | &check;      |
| statelessDefaultActions         | List<String>                      | &check;      |
| statelessFragmentDefaultActions | List<String>                      | &check;      |
| statelessRuleGroupReferences    | List<StatelessRuleGroupReference> | &check;      |

#### ActionDefinition
| **Name**            | **Type**            | **Nullable** |
| ------------------- | ------------------- | ------------ |
| publishMetricAction | PublishMetricAction | &check;      |

#### CustomAction
| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| actionDefinition | ActionDefinition | &check;      |
| actionName       | String           | &check;      |

#### Dimension
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| value    | String   | &check;      |

#### PublishMetricAction
| **Name**   | **Type**        | **Nullable** |
| ---------- | --------------- | ------------ |
| dimensions | List<Dimension> | &check;      |

#### StatefulEngineOptions
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| ruleOrder | String   | &check;      |

#### StatefulRuleGroupOverride
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| action   | String   | &check;      |

#### StatefulRuleGroupReference
| **Name**    | **Type**                  | **Nullable** |
| ----------- | ------------------------- | ------------ |
| override    | StatefulRuleGroupOverride | &check;      |
| priority    | Int                       | &check;      |
| resourceArn | String                    | &check;      |

#### StatelessRuleGroupReference
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| priority    | Int      | &check;      |
| resourceArn | String   | &check;      |
