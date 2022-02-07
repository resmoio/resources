---
description: OpenSearch Domain
---

# aws_opensearch_domain

Schema
```
{
	accessPolicies: JSON,
	accountId: String,
	advancedOptions: Map<String,String>,
	advancedSecurityOptions: AdvancedSecurityOptions,
	arn: String,
	associatedPackages: List<AssociatedPackage>,
	autoTuneOptions: AutoTuneOptionsOutput,
	clusterConfig: ClusterConfig,
	cognitoOptions: CognitoOptions,
	created: Boolean,
	deleted: Boolean,
	domainEndpointOptions: DomainEndpointOptions,
	domainId: String,
	domainName: String,
	ebsOptions: EBSOptions,
	encryptionAtRestOptions: EncryptionAtRestOptions,
	endpoint: String,
	endpoints: Map<String,String>,
	engineVersion: String,
	logPublishingOptions: Map<String,LogPublishingOption>,
	nodeToNodeEncryptionOptions: NodeToNodeEncryptionOptions,
	processing: Boolean,
	region: String,
	serviceSoftwareOptions: ServiceSoftwareOptions,
	snapshotOptions: SnapshotOptions,
	tags: Map<String,String>,
	upgradeProcessing: Boolean,
	vpcOptions: VPCDerivedInfo,
}
```
