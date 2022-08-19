---
description: Amazon Web Services Inspector Assessment Template
---
aws_inspector_assessment_template
---------------------------------

| **Name**                  | **Type**           | **Nullable** |
| ------------------------- | ------------------ | ------------ |
| accountId                 | String             | &cross;      |
| accountName               | String             | &check;      |
| arn                       | String             | &cross;      |
| assessmentTargetArn       | String             | &check;      |
| createdAt                 | String             | &check;      |
| durationInSeconds         | Int                | &check;      |
| lastAssessmentRunArn      | String             | &check;      |
| name                      | String             | &check;      |
| rulesPackageArns          | List<String>       | &check;      |
| userAttributesForFindings | Map<String,String> | &check;      |
