---
description: aws_backup_backup_job
---

# Backup Job

Schema
```
{
	accountId: String,
	backupJobAccountId: String,
	backupOptions: Map<String,String>,
	backupSizeInBytes: Long,
	backupType: String,
	backupVaultArn: String,
	backupVaultName: String,
	bytesTransferred: Long,
	completionDate: Date,
	createdBy: RecoveryPointCreator,
	creationDate: Date,
	expectedCompletionDate: Date,
	iamRoleArn: String,
	id: String,
	percentDone: String,
	recoveryPointArn: String,
	region: String,
	resourceArn: String,
	resourceType: String,
	startBy: Date,
	state: String,
	statusMessage: String,
}
```
