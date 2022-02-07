---
description: WAF V2 Web ACL
---

# aws_wafv2_web_acl

Schema
```
{
	accountId: String,
	arn: String,
	capacity: Long,
	captchaConfig: CaptchaConfig,
	customResponseBodies: Map<String,CustomResponseBody>,
	defaultAction: JSON,
	description: String,
	id: String,
	labelNamespace: String,
	managedByFirewallManager: Boolean,
	name: String,
	postProcessFirewallManagerRuleGroups: List<FirewallManagerRuleGroup>,
	preProcessFirewallManagerRuleGroups: List<FirewallManagerRuleGroup>,
	region: String,
	rules: List<Rule>,
	visibilityConfig: VisibilityConfig,
}
```
