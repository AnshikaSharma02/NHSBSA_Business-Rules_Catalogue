# DMN Rule Definition Document

## 1. Document Metadata
- **Document Title:** Business Rule for Activity Management 
- **Version:** 1.0
- **Author:** [Author Name]
- **Date:** 2024-08-08
- **Reviewers:** Ajit Dixit 
- **Approval Status:** Approved

## 2. DMN Rule Information
- **DMN Rule version number:** 01
- **DMN Rule Name:** DR-ACM-NHS_Num_Valid-0006
- ** **Effective from data:** 01/01/2023
- **Effective to date:** none
- **DMN Rule Description:** This business rule aims to check whether the Nhs num is valid or not based on certain conditions.
- **Business Owner:** Mark Yarnton
- **Rule Conditions:**
  - **Condition 1:** : It is going to check the Eligible for Ortho Reform, where the Activity claims, Regions and Apply for ortho reform check would be checked as per the business rule. 
  - **Condition 2:** The Date check is going to validate the Ortho reform start date, Date of Assessment and Date of Completion. 
- **Rule Actions:**
  - **Action 1:** Activity Claim --> FP17O, Apply for ortho reform check --> Y, Region --> England
  - **Action 2:** Date of Assessment or Date of Completion should be on or after the Ortho Reform start date. 
- **Rule Author:** Anshika Sharma 

## 3. DMN Rule Assets
### 3.1 DMN Model 
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

## 4. Dependencies
- **Included Model Name:**
- **Invoked Decision Service**
-**DMN asset link:** [Link to included DMN asset]

## 5. Exception Scenario
- **<<Add any exception scenario>>**

## 6. Traceability Matrix

 | Policy ID | DMN Model ID |  DMN MOdel Link                            | Stakeholder  | Status  |
 |-----------|--------------|--------------------------------------------|--------------|-------- |
 | -         | DS-ACM-0006  |  KIE Sandbox :: NHS_Number_Validation.dmn  | Stakeholder1 | Active  |

## 7. Change Log

| Version | Date       | Author        | Description of Changes            |
|---------|------------|---------------|-----------------------------------|
| 1.0     | 2024-08-08 | Anshika Sharma| Initial creation                  |
