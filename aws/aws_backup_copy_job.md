---
description: Backup Copy Job
---

# aws_backup_copy_job

Schema
```
{
	accountId: String,
	backupSizeInBytes: Long,
	completionDate: Date,
	copyJobAccountId: String,
	createdBy: RecoveryPointCreator,
	creationDate: Date,
	destinationBackupVaultArn: String,
	destinationRecoveryPointArn: String,
	iamRoleArn: String,
	id: String,
	region: String,
	resourceArn: String,
	resourceType: String,
	sourceBackupVaultArn: String,
	sourceRecoveryPointArn: String,
	state: String,
	statusMessage: String,
}
```
