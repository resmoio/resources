---
description: Project
---

# jira_project

Schema
```
{
	archived: Boolean,
	archivedBy: String,
	archivedDate: String,
	assigneeType: String,
	components: List<Component>,
	deleted: Boolean,
	deletedBy: String,
	deletedDate: String,
	description: String,
	favourite: Boolean,
	id: Int,
	insight: Insight,
	isPrivate: Boolean,
	issueTypes: List<IssueType>,
	key: String,
	lead: String,
	name: String,
	permissionScheme: PermissionScheme,
	projectCategory: Category,
	projectKeys: List<String>,
	projectTypeKey: String,
	retentionTillDate: String,
	roles: List<String>,
	simplified: Boolean,
	site: String,
	style: String,
	uuid: String,
	versions: List<Version>,
}
```
