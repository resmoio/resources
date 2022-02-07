---
description: Browser Application
---

# newrelic_browser_application

Schema
```
{
	accountId: Int,
	agentInstallType: String,
	alertSeverity: String,
	applicationId: Long,
	browserSettings: Setting,
	entityType: String,
	guid: String,
	indexedAt: Date,
	metricNormalizationRules: List<MetricNormalizationRule>,
	name: String,
	reporting: Boolean,
	runningAgentVersions: RunningAgentVersion,
	servingApmApplicationId: Int,
	settings: Setting,
	tags: List<Tag>,
	type: String,
}
```
