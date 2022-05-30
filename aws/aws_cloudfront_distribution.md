---
description: Amazon Web Services CloudFront Distribution
---
aws_cloudfront_distribution
---------------------------

| **Name**             | **Type**                  | **Nullable** |
| -------------------- | ------------------------- | ------------ |
| accountId            | String                    | &cross;      |
| aliasICPRecordals    | List<AliasICPRecordal>    | &check;      |
| aliases              | List<String>              | &cross;      |
| arn                  | String                    | &cross;      |
| cacheBehaviors       | List<CacheBehavior>       | &check;      |
| comment              | String                    | &check;      |
| customErrorResponses | List<CustomErrorResponse> | &check;      |
| defaultCacheBehavior | CacheBehavior             | &check;      |
| defaultRootObject    | String                    | &check;      |
| domainName           | String                    | &cross;      |
| enabled              | Boolean                   | &check;      |
| httpVersion          | String                    | &cross;      |
| id                   | String                    | &cross;      |
| isIPV6Enabled        | Boolean                   | &check;      |
| lastModifiedTime     | String                    | &check;      |
| logging              | LoggingConfig             | &check;      |
| originGroups         | List<OriginGroup>         | &check;      |
| origins              | List<Origin>              | &check;      |
| priceClass           | String                    | &check;      |
| restrictions         | GeoRestriction            | &check;      |
| status               | String                    | &cross;      |
| viewerCertificate    | ViewerCertificate         | &cross;      |
| webACLId             | String                    | &check;      |

#### AliasICPRecordal
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| cname             | String   | &check;      |
| icpRecordalStatus | String   | &check;      |

#### AllowedMethods
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| cachedMethods | List<String> | &cross;      |
| items         | List<String> | &cross;      |

#### CacheBehavior
| **Name**                   | **Type**                        | **Nullable** |
| -------------------------- | ------------------------------- | ------------ |
| allowedMethods             | AllowedMethods                  | &check;      |
| cachePolicyId              | String                          | &check;      |
| compress                   | Boolean                         | &check;      |
| fieldLevelEncryptionId     | String                          | &cross;      |
| functionAssociations       | List<FunctionAssociation>       | &check;      |
| lambdaFunctionAssociations | List<LambdaFunctionAssociation> | &check;      |
| originRequestPolicyId      | String                          | &check;      |
| pathPattern                | String                          | &check;      |
| realtimeLogConfigArn       | String                          | &check;      |
| responseHeadersPolicyId    | String                          | &check;      |
| smoothStreaming            | Boolean                         | &check;      |
| targetOriginId             | String                          | &cross;      |
| trustedKeyGroups           | TrustedKeyGroups                | &check;      |
| trustedSigners             | TrustedSigners                  | &check;      |
| viewerProtocolPolicy       | String                          | &check;      |

#### CustomErrorResponse
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| errorCachingMinTTL | Long     | &cross;      |
| errorCode          | Int      | &cross;      |
| responseCode       | String   | &cross;      |
| responsePagePath   | String   | &cross;      |

#### CustomOriginConfig
| **Name**               | **Type**     | **Nullable** |
| ---------------------- | ------------ | ------------ |
| httpPort               | Int          | &check;      |
| httpsPort              | Int          | &check;      |
| originKeepaliveTimeout | Int          | &check;      |
| originProtocolPolicy   | String       | &cross;      |
| originReadTimeout      | Int          | &check;      |
| originSslProtocols     | List<String> | &check;      |

#### FunctionAssociation
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| eventType   | String   | &cross;      |
| functionARN | String   | &cross;      |

#### GeoRestriction
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| items           | List<String> | &check;      |
| restrictionType | String       | &check;      |

#### Header
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| headerName  | String   | &cross;      |
| headerValue | String   | &cross;      |

#### LambdaFunctionAssociation
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| eventType         | String   | &cross;      |
| includeBody       | Boolean  | &cross;      |
| lambdaFunctionARN | String   | &cross;      |

#### LoggingConfig
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| bucket         | String   | &check;      |
| enabled        | Boolean  | &check;      |
| includeCookies | Boolean  | &check;      |
| prefix         | String   | &check;      |

#### Origin
| **Name**           | **Type**           | **Nullable** |
| ------------------ | ------------------ | ------------ |
| connectionAttempts | Int                | &check;      |
| connectionTimeout  | Int                | &check;      |
| customHeaders      | List<Header>       | &check;      |
| customOriginConfig | CustomOriginConfig | &check;      |
| domainName         | String             | &cross;      |
| id                 | String             | &cross;      |
| originPath         | String             | &cross;      |
| originShield       | OriginShield       | &check;      |
| s3OriginConfig     | String             | &check;      |

#### OriginGroup
| **Name**         | **Type**     | **Nullable** |
| ---------------- | ------------ | ------------ |
| failoverCriteria | List<Int>    | &check;      |
| id               | String       | &cross;      |
| members          | List<String> | &check;      |

#### OriginShield
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| enabled            | Boolean  | &check;      |
| originShieldRegion | String   | &check;      |

#### TrustedKeyGroups
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| enabled  | Boolean      | &cross;      |
| items    | List<String> | &cross;      |

#### TrustedSigners
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| enabled  | Boolean      | &cross;      |
| items    | List<String> | &cross;      |

#### ViewerCertificate
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| acmCertificateArn            | String   | &check;      |
| cloudFrontDefaultCertificate | Boolean  | &check;      |
| iamCertificateId             | String   | &check;      |
| minimumProtocolVersion       | String   | &check;      |
| sslSupportMethod             | String   | &check;      |
