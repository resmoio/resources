---
description: aws_backup_vault
---

# Backup Vault

Schema
```
{
	accessPolicy: JSON,
	accountId: String,
	arn: String,
	creationDate: Date,
	creatorRequestId: String,
	encryptionKeyArn: String,
	lockDate: Date,
	locked: Boolean,
	maxRetentionDays: Long,
	minRetentionDays: Long,
	name: String,
	notification: Notification,
	numberOfRecoveryPoints: Long,
	region: String,
	tags: Map<String,String>,
}
```
