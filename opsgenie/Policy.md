---
description: opsgenie_policy
---

# Policy

Schema
```
{
	alias: String,
	autoCloseAction: AutoCloseAction,
	autoRestartAction: AutoRestartAction,
	continue: Boolean,
	deduplicationAction: DeduplicationAction,
	delayAction: DelayAction,
	description: String,
	enabled: Boolean,
	filter: Filter,
	id: String,
	ignoreOriginalResponders: Boolean,
	ignoreOriginalTags: Boolean,
	message: String,
	name: String,
	order: Int,
	policyDescription: String,
	responders: List<Responder>,
	scope: String,
	suppress: Boolean,
	tags: List<String>,
	teamId: String,
	timeRestrictions: TimeRestrictions,
	type: String,
}
```
