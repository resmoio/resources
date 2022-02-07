---
description: Integration
---

# opsgenie_integration

Schema
```
{
	alertActions: List<String>,
	alertFilter: AlertFilter,
	allowConfigurationAccess: Boolean,
	allowDeleteAccess: Boolean,
	allowReadAccess: Boolean,
	allowWriteAccess: Boolean,
	enabled: Boolean,
	id: String,
	ignoreRespondersFromPayload: Boolean,
	ignoreTeamsFromPayload: Boolean,
	isAdvanced: Boolean,
	isGlobal: Boolean,
	name: String,
	responders: List<Responder>,
	sendAlertActions: Boolean,
	suppressNotifications: Boolean,
	type: String,
}
```
