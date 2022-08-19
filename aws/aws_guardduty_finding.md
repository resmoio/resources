---
description: Amazon Web Services GuardDuty Finding
---
aws_guardduty_finding
---------------------

| **Name**         | **Type**                    | **Nullable** |
| ---------------- | --------------------------- | ------------ |
| accountId        | String                      | &cross;      |
| accountName      | String                      | &check;      |
| arn              | String                      | &cross;      |
| confidence       | Double                      | &check;      |
| createdAt        | String                      | &check;      |
| description      | String                      | &check;      |
| findingAccountId | String                      | &cross;      |
| id               | String                      | &check;      |
| partition        | String                      | &check;      |
| region           | String                      | &check;      |
| resource         | AWSGuardDutyFindingResource | &check;      |
| schemaVersion    | String                      | &check;      |
| service          | Service                     | &check;      |
| severity         | Double                      | &check;      |
| title            | String                      | &check;      |
| type             | String                      | &check;      |
| updatedAt        | String                      | &check;      |

#### AWSGuardDutyFindingResource
| **Name**          | **Type**             | **Nullable** |
| ----------------- | -------------------- | ------------ |
| accessKeyDetails  | AccessKeyDetails     | &check;      |
| eksClusterDetails | EksClusterDetails    | &check;      |
| instanceDetails   | InstanceDetails      | &check;      |
| kubernetesDetails | KubernetesDetails    | &check;      |
| resourceType      | String               | &check;      |
| s3BucketDetails   | List<S3BucketDetail> | &check;      |

#### AccessControlList
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| allowsPublicReadAccess  | Boolean  | &check;      |
| allowsPublicWriteAccess | Boolean  | &check;      |

#### AccessKeyDetails
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| accessKeyId | String   | &check;      |
| principalId | String   | &check;      |
| userName    | String   | &check;      |
| userType    | String   | &check;      |

#### AccountLevelPermissions
| **Name**          | **Type**          | **Nullable** |
| ----------------- | ----------------- | ------------ |
| blockPublicAccess | BlockPublicAccess | &check;      |

#### Action
| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| actionType              | String                  | &check;      |
| awsApiCallAction        | AwsApiCallAction        | &check;      |
| dnsRequestAction        | DnsRequestAction        | &check;      |
| kubernetesApiCallAction | KubernetesApiCallAction | &check;      |
| networkConnectionAction | NetworkConnectionAction | &check;      |
| portProbeAction         | PortProbeAction         | &check;      |

#### AwsApiCallAction
| **Name**             | **Type**             | **Nullable** |
| -------------------- | -------------------- | ------------ |
| api                  | String               | &check;      |
| callerType           | String               | &check;      |
| domainDetails        | DomainDetails        | &check;      |
| errorCode            | String               | &check;      |
| remoteAccountDetails | RemoteAccountDetails | &check;      |
| remoteIpDetails      | RemoteIpDetails      | &check;      |
| serviceName          | String               | &check;      |
| userAgent            | String               | &check;      |

#### BlockPublicAccess
| **Name**              | **Type** | **Nullable** |
| --------------------- | -------- | ------------ |
| blockPublicAcls       | Boolean  | &check;      |
| blockPublicPolicy     | Boolean  | &check;      |
| ignorePublicAcls      | Boolean  | &check;      |
| restrictPublicBuckets | Boolean  | &check;      |

#### BucketLevelPermissions
| **Name**          | **Type**          | **Nullable** |
| ----------------- | ----------------- | ------------ |
| accessControlList | AccessControlList | &check;      |
| blockPublicAccess | BlockPublicAccess | &check;      |
| bucketPolicy      | BucketPolicy      | &check;      |

#### BucketPolicy
| **Name**                | **Type** | **Nullable** |
| ----------------------- | -------- | ------------ |
| allowsPublicReadAccess  | Boolean  | &check;      |
| allowsPublicWriteAccess | Boolean  | &check;      |

#### City
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| cityName | String   | &check;      |

#### Container
| **Name**         | **Type**          | **Nullable** |
| ---------------- | ----------------- | ------------ |
| containerRuntime | String            | &check;      |
| id               | String            | &check;      |
| image            | String            | &check;      |
| imagePrefix      | String            | &check;      |
| name             | String            | &check;      |
| securityContext  | SecurityContext   | &check;      |
| volumeMounts     | List<VolumeMount> | &check;      |

#### Country
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| countryCode | String   | &check;      |
| countryName | String   | &check;      |

#### DefaultServerSideEncryption
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| encryptionType  | String   | &check;      |
| kmsMasterKeyArn | String   | &check;      |

#### DnsRequestAction
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &check;      |

#### DomainDetails
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| domain   | String   | &check;      |

#### EksClusterDetails
| **Name**  | **Type**           | **Nullable** |
| --------- | ------------------ | ------------ |
| arn       | String             | &check;      |
| createdAt | String             | &check;      |
| name      | String             | &check;      |
| status    | String             | &check;      |
| tags      | Map<String,String> | &check;      |
| vpcId     | String             | &check;      |

#### Evidence
| **Name**                  | **Type**                       | **Nullable** |
| ------------------------- | ------------------------------ | ------------ |
| threatIntelligenceDetails | List<ThreatIntelligenceDetail> | &check;      |

#### GeoLocation
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| lat      | Double   | &check;      |
| lon      | Double   | &check;      |

#### HostPath
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| path     | String   | &check;      |

#### IamInstanceProfile
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| arn      | String   | &check;      |
| id       | String   | &check;      |

#### InstanceDetails
| **Name**           | **Type**               | **Nullable** |
| ------------------ | ---------------------- | ------------ |
| availabilityZone   | String                 | &check;      |
| iamInstanceProfile | IamInstanceProfile     | &check;      |
| imageDescription   | String                 | &check;      |
| imageId            | String                 | &check;      |
| instanceId         | String                 | &check;      |
| instanceState      | String                 | &check;      |
| instanceType       | String                 | &check;      |
| launchTime         | String                 | &check;      |
| networkInterfaces  | List<NetworkInterface> | &check;      |
| outpostArn         | String                 | &check;      |
| platform           | String                 | &check;      |
| productCodes       | List<ProductCode>      | &check;      |
| tags               | Map<String,String>     | &check;      |

#### KubernetesApiCallAction
| **Name**        | **Type**        | **Nullable** |
| --------------- | --------------- | ------------ |
| parameters      | String          | &check;      |
| remoteIpDetails | RemoteIpDetails | &check;      |
| requestUri      | String          | &check;      |
| sourceIps       | List<String>    | &check;      |
| statusCode      | Int             | &check;      |
| userAgent       | String          | &check;      |
| verb            | String          | &check;      |

#### KubernetesDetails
| **Name**                  | **Type**                  | **Nullable** |
| ------------------------- | ------------------------- | ------------ |
| kubernetesUserDetails     | KubernetesUserDetails     | &check;      |
| kubernetesWorkloadDetails | KubernetesWorkloadDetails | &check;      |

#### KubernetesUserDetails
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| groups   | List<String> | &check;      |
| uid      | String       | &check;      |
| username | String       | &check;      |

#### KubernetesWorkloadDetails
| **Name**    | **Type**        | **Nullable** |
| ----------- | --------------- | ------------ |
| containers  | List<Container> | &check;      |
| hostNetwork | Boolean         | &check;      |
| name        | String          | &check;      |
| namespace   | String          | &check;      |
| type        | String          | &check;      |
| uid         | String          | &check;      |
| volumes     | List<Volume>    | &check;      |

#### LocalIpDetails
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| ipAddressV4 | String   | &check;      |

#### LocalPortDetails
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| port     | Int      | &check;      |
| portName | String   | &check;      |

#### NetworkConnectionAction
| **Name**            | **Type**          | **Nullable** |
| ------------------- | ----------------- | ------------ |
| blocked             | Boolean           | &check;      |
| connectionDirection | String            | &check;      |
| localIpDetails      | LocalIpDetails    | &check;      |
| localPortDetails    | LocalPortDetails  | &check;      |
| protocol            | String            | &check;      |
| remoteIpDetails     | RemoteIpDetails   | &check;      |
| remotePortDetails   | RemotePortDetails | &check;      |

#### NetworkInterface
| **Name**           | **Type**                      | **Nullable** |
| ------------------ | ----------------------------- | ------------ |
| ipv6Addresses      | List<String>                  | &check;      |
| networkInterfaceId | String                        | &check;      |
| privateDnsName     | String                        | &check;      |
| privateIpAddress   | String                        | &check;      |
| privateIpAddresses | List<PrivateIpAddressDetails> | &check;      |
| publicDnsName      | String                        | &check;      |
| publicIp           | String                        | &check;      |
| securityGroups     | List<SecurityGroup>           | &check;      |
| subnetId           | String                        | &check;      |
| vpcId              | String                        | &check;      |

#### Organization
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| asn      | String   | &check;      |
| asnOrg   | String   | &check;      |
| isp      | String   | &check;      |
| org      | String   | &check;      |

#### Owner
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| id       | String   | &check;      |

#### PermissionConfiguration
| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| accountLevelPermissions | AccountLevelPermissions | &check;      |
| bucketLevelPermissions  | BucketLevelPermissions  | &check;      |

#### PortProbeAction
| **Name**         | **Type**              | **Nullable** |
| ---------------- | --------------------- | ------------ |
| blocked          | Boolean               | &check;      |
| portProbeDetails | List<PortProbeDetail> | &check;      |

#### PortProbeDetail
| **Name**         | **Type**         | **Nullable** |
| ---------------- | ---------------- | ------------ |
| localIpDetails   | LocalIpDetails   | &check;      |
| localPortDetails | LocalPortDetails | &check;      |
| remoteIpDetails  | RemoteIpDetails  | &check;      |

#### PrivateIpAddressDetails
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| privateDnsName   | String   | &check;      |
| privateIpAddress | String   | &check;      |

#### ProductCode
| **Name**    | **Type** | **Nullable** |
| ----------- | -------- | ------------ |
| code        | String   | &check;      |
| productType | String   | &check;      |

#### PublicAccess
| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| effectivePermission     | String                  | &check;      |
| permissionConfiguration | PermissionConfiguration | &check;      |

#### RemoteAccountDetails
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| accountId  | String   | &check;      |
| affiliated | Boolean  | &check;      |

#### RemoteIpDetails
| **Name**     | **Type**     | **Nullable** |
| ------------ | ------------ | ------------ |
| city         | City         | &check;      |
| country      | Country      | &check;      |
| geoLocation  | GeoLocation  | &check;      |
| ipAddressV4  | String       | &check;      |
| organization | Organization | &check;      |

#### RemotePortDetails
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| port     | Int      | &check;      |
| portName | String   | &check;      |

#### S3BucketDetail
| **Name**                    | **Type**                    | **Nullable** |
| --------------------------- | --------------------------- | ------------ |
| arn                         | String                      | &check;      |
| createdAt                   | String                      | &check;      |
| defaultServerSideEncryption | DefaultServerSideEncryption | &check;      |
| name                        | String                      | &check;      |
| owner                       | Owner                       | &check;      |
| publicAccess                | PublicAccess                | &check;      |
| tags                        | Map<String,String>          | &check;      |
| type                        | String                      | &check;      |

#### SecurityContext
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| privileged | Boolean  | &check;      |

#### SecurityGroup
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| groupId   | String   | &check;      |
| groupName | String   | &check;      |

#### Service
| **Name**       | **Type** | **Nullable** |
| -------------- | -------- | ------------ |
| action         | Action   | &check;      |
| archived       | Boolean  | &check;      |
| count          | Int      | &check;      |
| detectorId     | String   | &check;      |
| eventFirstSeen | String   | &check;      |
| eventLastSeen  | String   | &check;      |
| evidence       | Evidence | &check;      |
| resourceRole   | String   | &check;      |
| serviceName    | String   | &check;      |
| userFeedback   | String   | &check;      |

#### ThreatIntelligenceDetail
| **Name**       | **Type**     | **Nullable** |
| -------------- | ------------ | ------------ |
| threatListName | String       | &check;      |
| threatNames    | List<String> | &check;      |

#### Volume
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| hostPath | HostPath | &check;      |
| name     | String   | &check;      |

#### VolumeMount
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| mountPath | String   | &check;      |
| name      | String   | &check;      |
