# DMN Rule Definition Document

## 1. Document Metadata
- **Document Title:** NHS number validation rule for Activity Management 
- **Version:** 1.0
- **Author:** [Author Name]
- **Date:** 2024-08-08
- **Reviewers:** Ajit Dixit 
- **Approval Status:** Approved

## 2. DMN Rule Information
- **DMN Rule version number:** 01
- **DMN Rule Name:** DR-ACM-NHS_Num_Valid-0006
- **Effective from data:** 01/01/2023
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
  - **Input 1:** FP17 data
  - **Outputs:**
  - **Output 1:** Pass / Fail
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
