# DMN Rule Definition Document

## 1. Document Metadata
- **Document Title:** Business Rule for Activity Management 
- **Version:** 1.0
- **Author:** [Author Name]
- **Date:** 2024-08-08
- **Reviewers:** Ajit Dixit 
- **Approval Status:** Approved

## 2. Domain Information 
- **Domain Name:** Activity Management
- **Domain Description:** NHS Number Validation Process 
- **Business Owner:** [Business Owner Name]
- **Stakeholders:** NHSBSA,

## 3. Policy Information(If applicable) 
- **Policy ID:** 
- **Policy Name:** [Policy Name]
- **Policy Description:** [Detailed Description]
- **Effective Date:** 2024-08-01
- **Policy Owner:** [Policy Owner Name]
- 
## 4. Rule Definition Information
- **Rule ID:** R006
- **Rule Definition Name:** NHS Number Validation
- **Link:** Activity business rules examples.docx (sharepoint.com)
- **Effective Date:** 2024-08-01
- **Business Owner:** Mark Yanton

## 5. DMN Rule Information
- **DMN Rule ID:** ACM006
- **DMN Rule Name:** DR-ACM-NHS_Num_Valid-0006
- **DMN Rule Description:** This business rule aims to check whether the Nhs num is valid or not based on certain conditions. 
- **Rule Conditions:**
  - **Condition 1:** : It is going to check the Eligible for Ortho Reform, where the Activity claims, Regions and Apply for ortho reform check would be checked as per the business rule. 
  - **Condition 2:** The Date check is going to validate the Ortho reform start date, Date of Assessment and Date of Completion. 
- **Rule Actions:**
  - **Action 1:** Activity Claim --> FP17O, Apply for ortho reform check --> Y, Region --> England
  - **Action 2:** Date of Assessment or Date of Completion should be on or after the Ortho Reform start date. 
- **Rule Author:** Anshika Sharma 

## 6. DMN Rule Assets
### 6.1 DMN Model 
- **DMN Model Name:** DR-ACM-NHS_Num_Valid-0006
- **Decision Table Name:** Validity 
  - **Input 1:** ApplyOrthoReformChecks
  - **Input 2:** ActivityClaim
  - **Input 3:** Regions
  - **Input 4:** DateOfAssessment
  - **Input 5:** DateOfCompletion
  - **Input 6:** OrthoReformStartDate
- **Outputs:**
  - **Output 1:** EligibleForOrthoReform
  - **Output 2:** DateCheck
  - **Output 3:** Validity (Final Output)
- **Decision Logic:**
  - **Condition 1:** Decision box 1(EligibleForOrthoReform) is going to evaluate whether the input parameters are in compliance with the DMN Rule Action 
  - **Condition 2:** Decision box 2(DateCheck) is going to evaluate the date condition for the Date Check parameter 
  - **Action 1:** Check the input parameters and showcase the result in Boolean for decision boxes 1(EligibleForOrthoReform) and Decision box 2(DateCheck)
  - **Action 2:** : If both the output parameters are satisfied then the DMN rule Validity (Output 3 or the final output) would be satisfied and the NHS num should be valid, Otherwise Invalid. 
- **<<this section can be repeated if more than 1 DMN models are used>>**

## 7. Dependencies
- **Included Model Name:**
- **Invoked Decision Service**
-**DMN asset link:** [Link to included DMN asset]

## 8. Exception Scenario
- **<<Add any exception scenario>>**

## 9. Traceability Matrix

 | Policy ID | DMN Model ID |  DMN MOdel Link                            | Stakeholder  | Status  |
 |-----------|--------------|--------------------------------------------|--------------|-------- |
 | -         | DS-ACM-0006  |  KIE Sandbox :: NHS_Number_Validation.dmn  | Stakeholder1 | Active  |

## 10. Change Log

| Version | Date       | Author        | Description of Changes            |
|---------|------------|---------------|-----------------------------------|
| 1.0     | 2024-08-08 | Anshika Sharma| Initial creation                  |
