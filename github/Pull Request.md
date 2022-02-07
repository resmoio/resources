---
description: github_pull_request
---

# Pull Request

Schema
```
{
	activeLockReason: String,
	additions: Long,
	assignee: User,
	assignees: List<User>,
	authorAssociation: String,
	autoMerge: String,
	base: Base,
	body: String,
	changedFiles: Long,
	closedAt: Date,
	comments: Long,
	commits: Long,
	createdAt: Date,
	deletions: Long,
	draft: Boolean,
	head: Head,
	id: Long,
	labels: List<Label>,
	locked: Boolean,
	maintainerCanModify: Boolean,
	mergeCommitSha: String,
	mergeable: Boolean,
	mergeableState: String,
	merged: Boolean,
	mergedAt: Date,
	mergedBy: User,
	milestone: Milestone,
	nodeId: String,
	number: Long,
	organizationId: String,
	rebaseable: Boolean,
	repositoryId: String,
	requestedReviewers: List<User>,
	requestedTeams: List<RequestedTeam>,
	reviewComments: Long,
	state: String,
	title: String,
	updatedAt: Date,
	user: User,
}
```
