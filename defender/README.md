Defender
========
Integrating your Microsoft Defender account with Resmo can provide valuable insights and enhance your organization's security posture. Microsoft Defender offers advanced threat protection and endpoint security solutions. By connecting Defender with Resmo, you can collect and analyze data related to browser extensions, certificate assessments, recommendations, software vulnerabilities, and more, enabling you to effectively manage and mitigate security risks.

Here are the key resources that Resmo collects from the Microsoft Defender API:

* Defender Browser Extension: Retrieve information about browser extensions installed on devices, including extension details such as ID, name, version, risk level, vendor, and installation time. This allows you to monitor and manage browser extensions to ensure they align with your organization's security policies.
* Defender Certificate Assessment: Access details about certificate assessments performed on devices, including information about certificate properties, validity, key usage, and associated RBAC (Role-Based Access Control) groups. This helps you evaluate the security and trustworthiness of certificates used within your environment.
* Defender Recommendation: Gather information about security recommendations provided by Microsoft Defender. This includes details about recommended actions, associated weaknesses, severity scores, vulnerabilities, related threats, remediation options, and impact metrics. With this data, you can prioritize and address security gaps in your systems effectively.
* Defender Software: Retrieve information about software installed on devices, including details such as software name, vendor, weaknesses, vulnerabilities, exploit availability, active alerts, and the number of exposed and installed machines. This allows you to assess the security posture of your software assets and take appropriate actions to mitigate risks.
* Defender Vulnerability: Access details about software vulnerabilities, including vulnerability names, descriptions, severity levels, CVSS scores, exploit availability, and exposure data. This enables you to identify and address critical vulnerabilities in your systems to minimize the risk of exploitation.

By leveraging Resmo's capabilities, you can perform various actions and gain insights from the collected Microsoft Defender data:

* Monitor and manage browser extensions to ensure they are secure and aligned with organizational policies.
* Evaluate and assess the trustworthiness of certificates used in your environment.
* Prioritize and address security recommendations to mitigate vulnerabilities and weaknesses.
* Assess the security posture of software assets and take actions to mitigate risks.
* Identify and address critical software vulnerabilities to reduce the risk of exploitation.

With Resmo, you can effectively manage and enhance the security of your organization by leveraging the power of Microsoft Defender's advanced threat protection capabilities.

| **Resources**          | **Key**                                                                   | **Supports Events** |
| ---------------------- | ------------------------------------------------------------------------- | ------------------- |
| Browser Extension      | [defender\_browser\_extension](defender\_browser\_extension.md)           |                     |
| Certificate Assessment | [defender\_certificate\_assessment](defender\_certificate\_assessment.md) |                     |
| Recommendation         | [defender\_recommendation](defender\_recommendation.md)                   |                     |
| Software               | [defender\_software](defender\_software.md)                               |                     |
| Vulnerability          | [defender\_vulnerability](defender\_vulnerability.md)                     |                     |
