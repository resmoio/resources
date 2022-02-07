---
description: Repository
---

# github_repo

Schema
```
{
	allowAutoMerge: Boolean,
	allowMergeCommit: Boolean,
	allowRebaseMerge: Boolean,
	allowSquashMerge: Boolean,
	archived: Boolean,
	createdAt: String,
	defaultBranch: String,
	deleteBranchOnMerge: Boolean,
	description: String,
	disabled: Boolean,
	fork: Boolean,
	forks: Long,
	forksCount: Long,
	fullName: String,
	hasDownloads: Boolean,
	hasIssues: Boolean,
	hasPages: Boolean,
	hasProjects: Boolean,
	hasWiki: Boolean,
	homepage: String,
	id: Long,
	isTemplate: Boolean,
	language: String,
	license: License,
	name: String,
	networkCount: Long,
	nodeId: String,
	openIssues: Long,
	openIssuesCount: Long,
	organization: Organization,
	organizationId: String,
	owner: Owner,
	parent: Repo,
	permissions: Permissions,
	private: Boolean,
	pushedAt: String,
	size: Long,
	source: Repo,
	stargazersCount: Long,
	subscribersCount: Long,
	tempCloneToken: String,
	templateRepository: Repo,
	topics: List<String>,
	updatedAt: String,
	visibility: String,
	watchers: Long,
	watchersCount: Long,
}
```
