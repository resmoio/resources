---
description: aws_cloudtrail_trail
---

# CloudTrail

Schema
```
{
	accountId: String,
	cloudWatchLogsLogGroupArn: String,
	cloudWatchLogsRoleArn: String,
	hasCustomEventSelectors: Boolean,
	hasInsightSelectors: Boolean,
	homeRegion: String,
	includeGlobalServiceEvents: Boolean,
	isMultiRegionTrail: Boolean,
	isOrganizationTrail: Boolean,
	kmsKeyId: String,
	logFileValidationEnabled: Boolean,
	name: String,
	s3BucketName: String,
	s3KeyPrefix: String,
	snsTopicARN: String,
	trailARN: String,
}
```
