---
description: Lambda Function
---

# aws_lambda_function

Schema
```
{
	accountId: String,
	architectures: List<String>,
	arn: String,
	codeSha256: String,
	codeSize: Long,
	deadLetterConfig: DeadLetterConfig,
	description: String,
	env: Map<String,String>,
	handler: String,
	imageConfig: ImageConfig,
	kmsKeyArn: String,
	layers: List<Layer>,
	masterArn: String,
	memorySize: Int,
	name: String,
	packageType: String,
	region: String,
	revisionId: String,
	role: String,
	runtime: String,
	signingJobArn: String,
	signingProfileVersionArn: String,
	timeout: Int,
	tracingConfig: TracingConfig,
	version: String,
	vpcConfig: VpcConfig,
}
```
