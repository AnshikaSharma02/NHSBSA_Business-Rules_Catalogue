# DMN Rule Definition Document

## 1. Document Metadata
- **Document Title:** Business Rule for [Domain]
- **Version:** 1.0
- **Author:** [Author Name]
- **Date:** 2024-08-08
- **Reviewers:** [Reviewer Names]
- **Approval Status:** Draft

## 2. Domain Information 
- **Domain Name:** [Domain Name]
- **Domain Description:** [Short Description]
- **Process Name:** [Process Name]
  
  **Note**: In process name , Sub-domain is required. 
- **Business Owner:** [Business Owner Name]
- **Stakeholders:**[ List of Stakeholders]

## 3. Policy Information(If applicable) 
- **Policy ID:** [Policy ID]
- **Policy Name:** [Policy Name]
- **Policy Description:** [Detailed Description]
- **Effective Date:** 2024-08-01
- **Policy Owner:** [Policy Owner Name]

## 4. Rule Definition Information
- **Rule Definition Name:** [Name]
- **Link:** [Link to Rule Definition document]
- **Effective Date:** 2024-08-01
- **Business Owner:** [Rule Definition Business Owner]

## 5. DMN Rule Information
- **DMN Rule ID:** [Rule Definition ID]
  
  **Note**: The DMN rule ID will follow a specific format, which includes the domain name and the corresponding rule 
number as listed in the document. For example, the ID "PYM001" is structured as follows: "PYM" denotes the domain 
name, Payment Management, and "001" represents the sequential rule number as it appears in the document.
- **DMN Rule Name:** [Rule Name]

  **Note:** According to the naming convention, the DMN rule name must be defined.
- **DMN Rule Description:** [Detailed Description]
- **Rule Conditions:**
  - **Condition 1:** [Condition Description]
  - **Condition 2:** [Condition Description]
- **Rule Actions:**
  - **Action 1:** [Action Description]
  - **Action 2:** [Action Description]
- **Rule Author:** [Rule Author Name]

## 6. DMN Rule Assets
### 6.1 DMN Model 
- **DMN Model Name:** [DMN Model Name]
- **Decision Table Name:** [Decision Table Name]
- - **Inputs:**
  - **Input 1:** [Input Description]
  - **Input 2:** [Input Description]
- **Outputs:**
  - **Output 1:** [Output Description]
  - **Output 2:** [Output Description]
- **Decision Logic:**
  - **Condition 1:** [Condition Description]
  - **Condition 2:** [Condition Description]
  - **Action 1:** [Action Description]
  - **Action 2:** [Action Description]
- **<<this section can be repeated if more than 1 DMN models are used>>**

## 7. Dependencies
- **Included Model Name:**
- **Invoked Decision Service**
-**DMN asset link:** [Link to included DMN asset]
  
  **Note**: In this section, specify dependencies if a DMN rule is split across multiple DMN files or if external functions or reusable code are invoked. Include all relevant dependencies or links to the DMN models involved.

## 8. Exception Scenario
- **<<Add any exception scenario>>**

## 9. Traceability Matrix

| Policy ID | DMN Model ID |  DMN Model link     | Stakeholder  | Status |
|-----------|--------------|---------------------|--------------|--------|
| P001      | DMN001       | [Link to DMN model] | Stakeholder1 | Active |

## 10. Change Log

| Version | Date       | Author        | Description of Changes            |
|---------|------------|---------------|-----------------------------------|
| 1.0     | 2024-08-08 | [Author Name] | Initial creation                  |
