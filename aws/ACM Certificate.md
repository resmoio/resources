---
description: aws_acm_certificate
---

# ACM Certificate

Schema
```
{
	accountId: String,
	certificateArn: String,
	certificateAuthorityArn: String,
	createdAt: String,
	domainName: String,
	extendedKeyUsages: List<String>,
	failureReason: String,
	importedAt: String,
	inUseBy: List<String>,
	issuedAt: String,
	issuer: String,
	keyAlgorithm: String,
	keyUsages: List<String>,
	notAfter: String,
	notBefore: String,
	options: String,
	region: String,
	renewalEligibility: String,
	revocationReason: String,
	revokedAt: String,
	serial: String,
	signatureAlgorithm: String,
	status: String,
	subject: String,
	subjectAlternativeNames: List<String>,
	type: String,
}
```
