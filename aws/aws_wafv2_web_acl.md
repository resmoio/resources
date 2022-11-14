---
description: Amazon Web Services WAF V2 Web ACL
---
aws_wafv2_web_acl
-----------------

| **Name**                             | **Type**                       | **Nullable** |
| ------------------------------------ | ------------------------------ | ------------ |
| accountId                            | String                         | &cross;      |
| accountName                          | String                         | &check;      |
| arn                                  | String                         | &cross;      |
| capacity                             | Long                           | &check;      |
| captchaConfig                        | CaptchaConfig                  | &check;      |
| customResponseBodies                 | Map<String,CustomResponseBody> | &check;      |
| defaultAction                        | JSON                           | &check;      |
| description                          | String                         | &check;      |
| id                                   | String                         | &cross;      |
| labelNamespace                       | String                         | &check;      |
| loggingConfiguration                 | LoggingConfiguration           | &check;      |
| managedByFirewallManager             | Boolean                        | &check;      |
| name                                 | String                         | &cross;      |
| postProcessFirewallManagerRuleGroups | List<FirewallManagerRuleGroup> | &check;      |
| preProcessFirewallManagerRuleGroups  | List<FirewallManagerRuleGroup> | &check;      |
| region                               | String                         | &check;      |
| rules                                | List<Rule>                     | &check;      |
| visibilityConfig                     | VisibilityConfig               | &check;      |

#### CaptchaConfig
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| immunityTimeProperty | Long     | &check;      |

#### CustomResponseBody
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| content     | String   | &check;      |
| contentType | String   | &check;      |

#### FirewallManagerRuleGroup
| **Name**                 | **Type**         | **Nullable** |
| ------------------------ | ---------------- | ------------ |
| firewallManagerStatement | JSON             | &check;      |
| name                     | String           | &cross;      |
| overrideAction           | JSON             | &check;      |
| priority                 | Int              | &cross;      |
| visibilityConfig         | VisibilityConfig | &check;      |

#### LoggingConfiguration
| **Name**                 | **Type**     | **Nullable** |
| ------------------------ | ------------ | ------------ |
| logDestinationConfigs    | List<String> | &check;      |
| loggingFilter            | JSON         | &check;      |
| managedByFirewallManager | Boolean      | &check;      |
| redactedFields           | List<JSON>   | &check;      |
| resourceArn              | String       | &check;      |

#### Rule
| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| action           | JSON             | &check;      |
| captchaConfig    | CaptchaConfig    | &check;      |
| name             | String           | &cross;      |
| overrideAction   | JSON             | &check;      |
| priority         | Int              | &cross;      |
| ruleLabels       | List<String>     | &check;      |
| statement        | JSON             | &check;      |
| visibilityConfig | VisibilityConfig | &check;      |

#### VisibilityConfig
| **Name**                 | **Type** | **Nullable** |
| ------------------------ | -------- | ------------ |
| cloudWatchMetricsEnabled | Boolean  | &check;      |
| metricName               | String   | &check;      |
| sampledRequestsEnabled   | Boolean  | &check;      |
