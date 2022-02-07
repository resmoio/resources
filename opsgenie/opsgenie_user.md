---
description: opsgenie_user
---

# User

Schema
```
{
	blocked: Boolean,
	contact: List<Contact>,
	createdAt: String,
	details: Map<String,List>,
	escalations: List<Escalation>,
	fullName: String,
	id: String,
	locale: String,
	role: Role,
	schedule: List<Schedule>,
	tags: List<String>,
	team: List<Team>,
	timeZone: String,
	userAddress: UserAddress,
	userForwardingRule: List<ForwardingRule>,
	username: String,
	verified: Boolean,
}
```
