---
description: aws_cloudfront_distribution
---

# CloudFront Distribution

Schema
```
{
	accountId: String,
	aliasICPRecordals: List<AliasICPRecordal>,
	aliases: List<String>,
	arn: String,
	cacheBehaviors: List<CacheBehavior>,
	comment: String,
	customErrorResponses: List<CustomErrorResponse>,
	defaultCacheBehavior: CacheBehavior,
	defaultRootObject: String,
	domainName: String,
	enabled: Boolean,
	httpVersion: String,
	id: String,
	isIPV6Enabled: Boolean,
	lastModifiedTime: String,
	logging: LoggingConfig,
	originGroups: List<OriginGroup>,
	origins: List<Origin>,
	priceClass: String,
	restrictions: GeoRestriction,
	status: String,
	viewerCertificate: ViewerCertificate,
	webACLId: String,
}
```
