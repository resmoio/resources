---
description: Notification Rule
---

# opsgenie_notification_rule

Schema
```
{
	actionType: String,
	id: String,
	name: String,
	notificationTime: List<String>,
	order: Int,
	schedules: List<Schedule>,
	steps: List<Step>,
	timeRestriction: TimeRestriction,
	userId: String,
}
```
