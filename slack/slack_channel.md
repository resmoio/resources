---
description: Channel
---

# slack_channel

Schema
```
{
	connectedLimitedTeamIds: List<String>,
	connectedTeamIds: List<String>,
	conversationHostId: String,
	created: Int,
	creator: String,
	enterpriseId: String,
	globalShared: Boolean,
	id: String,
	internalTeamIds: List<String>,
	isArchived: Boolean,
	isChannel: Boolean,
	isExtShared: Boolean,
	isGeneral: Boolean,
	isGroup: Boolean,
	isIm: Boolean,
	isMember: Boolean,
	isMoved: Int,
	isMpim: Boolean,
	isNonThreadable: Boolean,
	isOrgShared: Boolean,
	isPendingExtShared: Boolean,
	isPrivate: Boolean,
	isReadOnly: Boolean,
	isShared: Boolean,
	isThreadOnly: Boolean,
	isUserDeleted: Boolean,
	locale: String,
	name: String,
	nameNormalized: String,
	open: Boolean,
	orgDefault: Boolean,
	orgMandatory: Boolean,
	parentConversation: String,
	pendingConnectedTeamIds: List<String>,
	pendingShared: List<String>,
	previousNames: List<String>,
	priority: Double,
	purpose: Topic,
	sharedTeamIds: List<String>,
	teamId: String,
	topic: Topic,
	unlinked: Int,
	user: String,
}
```
