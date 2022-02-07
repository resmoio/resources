---
description: Backup Plan
---

# aws_backup_plan

Schema
```
{
	accountId: String,
	advancedBackupSettings: List<AdvancedBackupSetting>,
	arn: String,
	creationDate: Date,
	creatorRequestId: String,
	deletionDate: Date,
	id: String,
	lastExecutionDate: Date,
	name: String,
	region: String,
	rules: List<BackupRule>,
	tags: Map<String,String>,
	versionId: String,
}
```
