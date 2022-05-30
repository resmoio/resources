---
description: Kubernetes Pod
---
kubernetes_pod
--------------

| **Name** | **Type**   | **Nullable** |
| -------- | ---------- | ------------ |
| metadata | ObjectMeta | &cross;      |
| spec     | PodSpec    | &check;      |
| status   | PodStatus  | &cross;      |

#### Affinity
| **Name**        | **Type**                 | **Nullable** |
| --------------- | ------------------------ | ------------ |
| nodeAffinity    | Affinity.NodeAffinity    | &check;      |
| podAffinity     | Affinity.PodAffinity     | &check;      |
| podAntiAffinity | Affinity.PodAntiAffinity | &check;      |

#### Affinity.NodeAffinity
| **Name**                                        | **Type**                               | **Nullable** |
| ----------------------------------------------- | -------------------------------------- | ------------ |
| preferredDuringSchedulingIgnoredDuringExecution | List<Affinity.PreferredSchedulingTerm> | &check;      |
| requiredDuringSchedulingIgnoredDuringExecution  | Affinity.NodeSelector                  | &check;      |

#### Affinity.NodeSelector
| **Name**          | **Type**                        | **Nullable** |
| ----------------- | ------------------------------- | ------------ |
| nodeSelectorTerms | List<Affinity.NodeSelectorTerm> | &check;      |

#### Affinity.NodeSelectorRequirement
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &check;      |
| operator | String       | &check;      |
| values   | List<String> | &check;      |

#### Affinity.NodeSelectorTerm
| **Name**         | **Type**                               | **Nullable** |
| ---------------- | -------------------------------------- | ------------ |
| matchExpressions | List<Affinity.NodeSelectorRequirement> | &check;      |
| matchFields      | List<Affinity.NodeSelectorRequirement> | &check;      |

#### Affinity.PodAffinity
| **Name**                                        | **Type**                               | **Nullable** |
| ----------------------------------------------- | -------------------------------------- | ------------ |
| preferredDuringSchedulingIgnoredDuringExecution | List<Affinity.WeightedPodAffinityTerm> | &check;      |
| requiredDuringSchedulingIgnoredDuringExecution  | List<Affinity.PodAffinityTerm>         | &check;      |

#### Affinity.PodAffinityTerm
| **Name**      | **Type**      | **Nullable** |
| ------------- | ------------- | ------------ |
| labelSelector | LabelSelector | &check;      |
| namespaces    | List<String>  | &check;      |
| topologyKey   | String        | &check;      |

#### Affinity.PodAntiAffinity
| **Name**                                        | **Type**                               | **Nullable** |
| ----------------------------------------------- | -------------------------------------- | ------------ |
| preferredDuringSchedulingIgnoredDuringExecution | List<Affinity.WeightedPodAffinityTerm> | &check;      |
| requiredDuringSchedulingIgnoredDuringExecution  | List<Affinity.PodAffinityTerm>         | &check;      |

#### Affinity.PreferredSchedulingTerm
| **Name**   | **Type**                  | **Nullable** |
| ---------- | ------------------------- | ------------ |
| preference | Affinity.NodeSelectorTerm | &check;      |
| weight     | Int                       | &check;      |

#### Affinity.WeightedPodAffinityTerm
| **Name**        | **Type**                 | **Nullable** |
| --------------- | ------------------------ | ------------ |
| podAffinityTerm | Affinity.PodAffinityTerm | &check;      |
| weight          | Int                      | &check;      |

#### BaseKubernetesResource
| **Name** | **Type** | **Nullable** || -------- | -------- | ------------ |


#### Container
| **Name**                 | **Type**                       | **Nullable** |
| ------------------------ | ------------------------------ | ------------ |
| args                     | List<String>                   | &check;      |
| command                  | List<String>                   | &check;      |
| image                    | String                         | &check;      |
| imagePullPolicy          | String                         | &check;      |
| livenessProbe            | Container.Probe                | &check;      |
| name                     | String                         | &check;      |
| ports                    | List<Container.ContainerPort>  | &check;      |
| readinessProbe           | Container.Probe                | &check;      |
| resources                | Container.ResourceRequirements | &check;      |
| securityContext          | Container.SecurityContext      | &check;      |
| stdin                    | Boolean                        | &check;      |
| stdinOnce                | Boolean                        | &check;      |
| terminationMessagePath   | String                         | &check;      |
| terminationMessagePolicy | String                         | &check;      |
| tty                      | Boolean                        | &check;      |
| volumeDevices            | List<Container.VolumeDevice>   | &check;      |
| volumeMounts             | List<Container.VolumeMount>    | &check;      |
| workingDir               | String                         | &check;      |

#### Container.Capabilities
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| add      | List<String> | &check;      |
| drop     | List<String> | &check;      |

#### Container.ContainerPort
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| containerPort | Int      | &check;      |
| hostIP        | String   | &check;      |
| hostPort      | Int      | &check;      |
| name          | String   | &check;      |
| protocol      | String   | &check;      |

#### Container.Probe
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| failureThreshold    | Int      | &check;      |
| handler             | JSON     | &check;      |
| initialDelaySeconds | Int      | &check;      |
| periodSeconds       | Int      | &check;      |
| successThreshold    | Int      | &check;      |
| timeoutSeconds      | Int      | &check;      |

#### Container.ResourceRequirements
| **Name** | **Type**           | **Nullable** |
| -------- | ------------------ | ------------ |
| limits   | Map<String,String> | &check;      |
| requests | Map<String,String> | &check;      |

#### Container.SELinuxOptions
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| level    | String   | &check;      |
| role     | String   | &check;      |
| type     | String   | &check;      |
| user     | String   | &check;      |

#### Container.SecurityContext
| **Name**                 | **Type**                                | **Nullable** |
| ------------------------ | --------------------------------------- | ------------ |
| allowPrivilegeEscalation | Boolean                                 | &check;      |
| capabilities             | Container.Capabilities                  | &check;      |
| privileged               | Boolean                                 | &check;      |
| procMount                | String                                  | &check;      |
| readOnlyRootFilesystem   | Boolean                                 | &check;      |
| runAsGroup               | Long                                    | &check;      |
| runAsNonRoot             | Boolean                                 | &check;      |
| runAsUser                | Long                                    | &check;      |
| seLinuxOptions           | Container.SELinuxOptions                | &check;      |
| windowsOptions           | Container.WindowsSecurityContextOptions | &check;      |

#### Container.VolumeDevice
| **Name**   | **Type** | **Nullable** |
| ---------- | -------- | ------------ |
| devicePath | String   | &check;      |
| name       | String   | &check;      |

#### Container.VolumeMount
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| mountPath        | String   | &check;      |
| mountPropagation | String   | &check;      |
| name             | String   | &check;      |
| readOnly         | Boolean  | &check;      |
| subPath          | String   | &check;      |
| subPathExpr      | String   | &check;      |

#### Container.WindowsSecurityContextOptions
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| gmsaCredentialSpec     | String   | &check;      |
| gmsaCredentialSpecName | String   | &check;      |
| runAsUserName          | String   | &check;      |

#### EphemeralContainer
| **Name**                 | **Type**                     | **Nullable** |
| ------------------------ | ---------------------------- | ------------ |
| args                     | List<String>                 | &check;      |
| command                  | List<String>                 | &check;      |
| image                    | String                       | &check;      |
| imagePullPolicy          | String                       | &check;      |
| name                     | String                       | &check;      |
| ports                    | Container.ContainerPort      | &check;      |
| securityContext          | Container.SecurityContext    | &check;      |
| stdin                    | Boolean                      | &check;      |
| stdinOnce                | Boolean                      | &check;      |
| targetContainerName      | String                       | &check;      |
| terminationMessagePath   | String                       | &check;      |
| terminationMessagePolicy | String                       | &check;      |
| tty                      | Boolean                      | &check;      |
| volumeDevices            | List<Container.VolumeDevice> | &check;      |
| volumeMounts             | List<Container.VolumeMount>  | &check;      |
| workingDir               | String                       | &check;      |

#### LabelSelector
| **Name**         | **Type**                        | **Nullable** |
| ---------------- | ------------------------------- | ------------ |
| matchExpressions | List<LabelSelector.Requirement> | &check;      |
| matchLabels      | Map<String,String>              | &check;      |

#### LabelSelector.Requirement
| **Name** | **Type**     | **Nullable** |
| -------- | ------------ | ------------ |
| key      | String       | &check;      |
| operator | String       | &check;      |
| values   | List<String> | &check;      |

#### ObjectMeta
| **Name**                   | **Type**                        | **Nullable** |
| -------------------------- | ------------------------------- | ------------ |
| annotations                | Map<String,String>              | &check;      |
| clusterName                | String                          | &check;      |
| creationTimestamp          | String                          | &check;      |
| deletionGracePeriodSeconds | Long                            | &check;      |
| deletionTimestamp          | String                          | &check;      |
| generateName               | String                          | &check;      |
| labels                     | Map<String,String>              | &check;      |
| name                       | String                          | &check;      |
| namespace                  | String                          | &check;      |
| ownerReferences            | List<ObjectMeta.OwnerReference> | &check;      |
| uid                        | String                          | &check;      |

#### ObjectMeta.OwnerReference
| **Name**           | **Type** | **Nullable** |
| ------------------ | -------- | ------------ |
| apiVersion         | String   | &check;      |
| blockOwnerDeletion | Boolean  | &check;      |
| controller         | Boolean  | &check;      |
| kind               | String   | &check;      |
| name               | String   | &check;      |
| uid                | String   | &check;      |

#### PodSpec
| **Name**                      | **Type**                   | **Nullable** |
| ----------------------------- | -------------------------- | ------------ |
| activeDeadlineSeconds         | Long                       | &check;      |
| affinity                      | Affinity                   | &check;      |
| containers                    | List<Container>            | &check;      |
| dnsConfig                     | PodSpec.PodDNSConfig       | &check;      |
| dnsPolicy                     | String                     | &check;      |
| ephemeralContainers           | List<EphemeralContainer>   | &check;      |
| hostAliases                   | List<PodSpec.HostAlias>    | &check;      |
| hostIPC                       | Boolean                    | &check;      |
| hostNetwork                   | Boolean                    | &check;      |
| hostPID                       | Boolean                    | &check;      |
| hostname                      | String                     | &check;      |
| initContainers                | List<Container>            | &check;      |
| nodeName                      | String                     | &check;      |
| nodeSelector                  | Map<String,String>         | &check;      |
| preemptionPolicy              | String                     | &check;      |
| priority                      | Int                        | &check;      |
| priorityClassName             | String                     | &check;      |
| restartPolicy                 | String                     | &check;      |
| runtimeClassName              | String                     | &check;      |
| schedulerName                 | String                     | &check;      |
| securityContext               | PodSpec.PodSecurityContext | &check;      |
| serviceAccount                | String                     | &check;      |
| serviceAccountName            | String                     | &check;      |
| shareProcessNamespace         | Boolean                    | &check;      |
| subdomain                     | String                     | &check;      |
| terminationGracePeriodSeconds | Long                       | &check;      |
| tolerations                   | List<PodSpec.Toleration>   | &check;      |
| volumes                       | List<JSON>                 | &check;      |

#### PodSpec.HostAlias
| **Name**  | **Type**     | **Nullable** |
| --------- | ------------ | ------------ |
| hostnames | List<String> | &check;      |
| ip        | String       | &check;      |

#### PodSpec.PodDNSConfig
| **Name**    | **Type**                                      | **Nullable** |
| ----------- | --------------------------------------------- | ------------ |
| nameservers | List<String>                                  | &check;      |
| options     | List<PodSpec.PodDNSConfig.PodDNSConfigOption> | &check;      |
| searches    | List<String>                                  | &check;      |

#### PodSpec.PodDNSConfig.PodDNSConfigOption
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| values   | String   | &check;      |

#### PodSpec.PodSecurityContext
| **Name**            | **Type**                                | **Nullable** |
| ------------------- | --------------------------------------- | ------------ |
| fsGroup             | Long                                    | &check;      |
| fsGroupChangePolicy | String                                  | &check;      |
| runAsGroup          | Long                                    | &check;      |
| runAsNonRoot        | Boolean                                 | &check;      |
| runAsUser           | Long                                    | &check;      |
| seLinuxOptions      | Container.SELinuxOptions                | &check;      |
| supplementalGroups  | List<Long>                              | &check;      |
| sysctls             | List<PodSpec.PodSecurityContext.Sysctl> | &check;      |
| windowsOptions      | Container.WindowsSecurityContextOptions | &check;      |

#### PodSpec.PodSecurityContext.Sysctl
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| name     | String   | &check;      |
| value    | String   | &check;      |

#### PodSpec.Toleration
| **Name**          | **Type** | **Nullable** |
| ----------------- | -------- | ------------ |
| effect            | String   | &check;      |
| key               | String   | &check;      |
| operator          | String   | &check;      |
| tolerationSeconds | Long     | &check;      |
| value             | String   | &check;      |

#### PodStatus
| **Name**          | **Type**              | **Nullable** |
| ----------------- | --------------------- | ------------ |
| hostIP            | String                | &check;      |
| message           | String                | &check;      |
| nominatedNodeName | String                | &check;      |
| podIP             | String                | &check;      |
| podIPs            | List<PodStatus.PodIP> | &check;      |
| qosClass          | String                | &check;      |
| startTime         | String                | &check;      |

#### PodStatus.PodIP
| **Name** | **Type** | **Nullable** |
| -------- | -------- | ------------ |
| ip       | String   | &check;      |

#### PodTemplateSpec
| **Name** | **Type**   | **Nullable** |
| -------- | ---------- | ------------ |
| metadata | ObjectMeta | &cross;      |
| spec     | PodSpec    | &cross;      |
