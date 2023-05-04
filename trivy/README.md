Trivy
=====
Integrating your Trivy account with Resmo enables you to gain valuable insights into your organization's vulnerability management and software supply chain security. Trivy is a comprehensive vulnerability scanner for containers and other artifacts, identifying security issues in your software components. By collecting and analyzing data from Trivy, Resmo can help you understand the vulnerabilities present in your software, enabling you to mitigate risks and maintain a secure environment.

With Resmo's SQL query capabilities, users can ask complex questions about their Trivy data:

* What are the details of each vulnerability detected, including its severity, description, affected components, and suggested fixes?
* How does the software bill of materials (SBOM) for each scanned artifact look, and what components are included in it?
* Which vulnerabilities have been recently published or updated, potentially indicating a need for immediate action?
* How do the severity levels of detected vulnerabilities vary across different software components and targets?
* Which CWEs (Common Weakness Enumerations) are most frequently associated with the identified vulnerabilities?

Setting up change alerts can be beneficial for monitoring critical changes in your Trivy data:

* Get notified when new vulnerabilities are detected in your software components, allowing you to take immediate action to address them.
* Receive an alert when the SBOM for an artifact changes, indicating modifications in the software supply chain that may require further investigation.
* Monitor updates to vulnerability information, such as new fixes or severity changes, to ensure timely response to potential threats.
* Stay informed about the addition or removal of components in your SBOM, which can impact your software's security posture.
* Track changes in CWE frequency to identify recurring patterns and prioritize efforts to mitigate specific types of vulnerabilities.

In conclusion, integrating your Trivy account with Resmo provides valuable insights into your organization's vulnerability management and software supply chain security. By leveraging Resmo's SQL query capabilities and change alerting, you can stay informed about potential security risks in your software components and take timely action to protect your organization from threats.

| **Resources** | **Key**                                         | **Supports Events** |
| ------------- | ----------------------------------------------- | ------------------- |
| SBOM          | [trivy\_sbom](trivy\_sbom.md)                   |                     |
| Vulnerability | [trivy\_vulnerability](trivy\_vulnerability.md) |                     |
