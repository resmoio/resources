---
description: gitlab_merge_request
---

# Merge Request

Schema
```
{
	approvalsBeforeMerge: String,
	assignee: User,
	assignees: List<User>,
	author: User,
	blockingDiscussionsResolved: Boolean,
	closedAt: Date,
	closedBy: String,
	createdAt: Date,
	description: String,
	discussionLocked: String,
	downvotes: Int,
	draft: Boolean,
	forceRemoveSourceBranch: Boolean,
	hasConflicts: Boolean,
	id: String,
	iid: Int,
	labels: List<String>,
	mergeCommitSha: String,
	mergeStatus: String,
	mergeWhenPipelineSucceeds: Boolean,
	mergedAt: Date,
	mergedBy: String,
	milestone: String,
	projectId: Int,
	reference: String,
	references: References,
	reviewers: List<User>,
	sha: String,
	shouldRemoveSourceBranch: String,
	sourceBranch: String,
	sourceProjectId: Int,
	squash: Boolean,
	squashCommitSha: String,
	state: String,
	targetBranch: String,
	targetProjectId: Int,
	taskCompletionStatus: TaskCompletionStatus,
	timeStats: TimeStats,
	title: String,
	updatedAt: Date,
	upvotes: Int,
	userNotesCount: Int,
	webUrl: String,
	workInProgress: Boolean,
}
```
