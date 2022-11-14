---
description: Amazon Web Services Network Firewall Rule Group
---
aws_networkfirewall_rule_group
------------------------------

| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| accountId               | String                  | &cross;      |
| accountName             | String                  | &check;      |
| arn                     | String                  | &cross;      |
| capacity                | Int                     | &check;      |
| consumedCapacity        | Int                     | &check;      |
| description             | String                  | &check;      |
| encryptionConfiguration | EncryptionConfiguration | &check;      |
| lastModifiedTime        | String                  | &check;      |
| name                    | String                  | &cross;      |
| numberOfAssociations    | Int                     | &check;      |
| referenceSets           | ReferenceSets           | &check;      |
| region                  | String                  | &cross;      |
| ruleGroupId             | String                  | &check;      |
| ruleGroupStatus         | String                  | &check;      |
| ruleVariables           | RuleVariables           | &check;      |
| rulesSource             | RulesSource             | &check;      |
| snsTopic                | String                  | &check;      |
| sourceMetadata          | SourceMetadata          | &check;      |
| statefulRuleOptions     | StatefulRuleOptions     | &check;      |
| tags                    | Map<String,String>      | &check;      |
| type                    | String                  | &check;      |

#### EncryptionConfiguration
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| keyId    | String   | &check;      |
| type     | String   | &check;      |

#### Header
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| destination     | String   | &check;      |
| destinationPort | String   | &check;      |
| direction       | String   | &check;      |
| protocol        | String   | &check;      |
| source          | String   | &check;      |
| sourcePort      | String   | &check;      |

#### ReferenceSets
| **Name**        | **Type**           | **Nullable** |
| --------------- | ------------------ | ------------ |
| ipSetReferences | Map<String,String> | &check;      |

#### RuleOption
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| keyword  | String       | &check;      |
| settings | List<String> | &check;      |

#### RuleVariables
| **Name** | **Type**         | **Nullable** |
| -------- | ---------------- | ------------ |
| ipSets   | Map<String,List> | &check;      |
| portSets | Map<String,List> | &check;      |

#### RulesSource
| **Name**                       | **Type**           | **Nullable** |
| ------------------------------ | ------------------ | ------------ |
| rulesSourceList                | RulesSourceList    | &check;      |
| rulesString                    | String             | &check;      |
| statefulRules                  | List<StatefulRule> | &check;      |
| statelessRulesAndCustomActions | JSON               | &check;      |

#### RulesSourceList
| **Name**           | **Type**     | **Nullable** |
| ------------------ | ------------ | ------------ |
| generatedRulesType | String       | &check;      |
| targetTypes        | List<String> | &check;      |
| targets            | List<String> | &check;      |

#### SourceMetadata
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| sourceArn         | String   | &check;      |
| sourceUpdateToken | String   | &check;      |

#### StatefulRule
| **Name**    | **Type**         | **Nullable** |
| ----------- | ---------------- | ------------ |
| action      | String           | &check;      |
| header      | Header           | &check;      |
| ruleOptions | List<RuleOption> | &check;      |

#### StatefulRuleOptions
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| ruleOrder | String   | &check;      |
