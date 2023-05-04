Kubernetes
==========
Connecting your Kubernetes cluster to Resmo can be beneficial in various ways. Kubernetes is a container orchestration platform that automates the deployment, scaling, and management of containerized applications. Resmo can collect and analyze configuration data from Kubernetes, which can be useful for identifying security risks, detecting best practices, and optimizing configurations.

Using Resmo's SQL query capabilities, users can ask complex questions about their Kubernetes configuration data. For example:

* Which pods are running on a specific node?
* How many replicas are configured for a particular deployment?
* What is the resource usage of services in a specific namespace?
* Which namespaces have the highest number of running pods?
* How many network policies are applied to a specific namespace?

Setting up change alerts can also be helpful for monitoring critical changes in your Kubernetes configuration. For example:

* Get notified when a new deployment is created in your Kubernetes cluster.
* Receive an alert when a pod's status changes to 'Error' or 'CrashLoopBackOff'.
* Get notified when a service's configuration is updated.
* Receive an alert when a new ingress resource is added to your cluster.
* Get notified when a role binding's permissions are modified.

In conclusion, connecting your Kubernetes cluster to Resmo can provide valuable insights into your organization's container orchestration and management. By leveraging Resmo's SQL query capabilities and change alerting, you can stay on top of important changes and optimize your Kubernetes configuration for maximum efficiency.

| **Resources**        | **Key**                                                                     | **Supports Events** |
| -------------------- | --------------------------------------------------------------------------- | ------------------- |
| Cluster Role         | [kubernetes\_cluster\_role](kubernetes\_cluster\_role.md)                   |                     |
| Cluster Role Binding | [kubernetes\_cluster\_role\_binding](kubernetes\_cluster\_role\_binding.md) |                     |
| Cron Job             | [kubernetes\_cron\_job](kubernetes\_cron\_job.md)                           |                     |
| DaemonSet            | [kubernetes\_daemonset](kubernetes\_daemonset.md)                           |                     |
| Deployment           | [kubernetes\_deployment](kubernetes\_deployment.md)                         |                     |
| Ingress              | [kubernetes\_ingress](kubernetes\_ingress.md)                               |                     |
| Job                  | [kubernetes\_job](kubernetes\_job.md)                                       |                     |
| Namespace            | [kubernetes\_namespace](kubernetes\_namespace.md)                           |                     |
| Network Policy       | [kubernetes\_network\_policy](kubernetes\_network\_policy.md)               |                     |
| Pod                  | [kubernetes\_pod](kubernetes\_pod.md)                                       |                     |
| ReplicaSet           | [kubernetes\_replicaset](kubernetes\_replicaset.md)                         |                     |
| Role                 | [kubernetes\_role](kubernetes\_role.md)                                     |                     |
| Role Binding         | [kubernetes\_role\_binding](kubernetes\_role\_binding.md)                   |                     |
| Service              | [kubernetes\_service](kubernetes\_service.md)                               |                     |
| StatefulSet          | [kubernetes\_statefulset](kubernetes\_statefulset.md)                       |                     |
