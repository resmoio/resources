---
description: github_issue
---

# Issue

Schema
```
{
	assignee: User,
	assignees: List<User>,
	authorAssociation: String,
	body: String,
	closedAt: Date,
	closedBy: User,
	comments: Int,
	createdAt: Date,
	id: Long,
	labels: List<Label>,
	locked: Boolean,
	milestone: Milestone,
	nodeId: String,
	number: Long,
	organizationId: String,
	repositoryId: String,
	state: String,
	title: String,
	updatedAt: Date,
	user: User,
}
```
