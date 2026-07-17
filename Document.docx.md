# Lead Capture & Validation Automation System

# Introduction

The **Lead Capture & Validation Automation System** is designed to automate the process of collecting leads, validating submitted information, detecting duplicate entries, storing valid records in the CRM, and sending confirmation emails. This document presents the QA testing conducted to verify that the workflow functions according to the project requirements.

# Objective

The objective of this document is to verify the functionality, reliability, and accuracy of the Lead Capture & Validation Automation System. The testing ensures that valid leads are processed successfully, invalid email addresses are handled correctly, duplicate submissions are identified, required fields are validated, and the automation workflow performs as expected.

# Test Environment

* **Google Forms** – Used for lead submission.   
* **Google Sheets** – Used to store form responses and CRM records.   
* **n8n** – Used to automate validation, duplicate detection, and workflow execution.   
* **Gmail** – Used for sending confirmation emails to valid leads.   
* **Web Browser** – Google Chrome.

|  |  |  |  |  |
| :---- | :---- | :---- | :---- | :---- |
|  |  |  |  |  |
|  |  |  |  |  |

| Test ID | Test Scenario | Expected Result | Actual Result | Status |
| :---: | :---: | :---: | :---: | :---: |
| TC-001 | Valid Lead Submission | Lead should be stored, workflow executed, confirmation email sent. | Workflow executed successfully, data stored in Google Sheets, confirmation email received. | PASS |
| TC-002 | Invalid Email | Invalid email should not receive confirmation email. | Workflow executed, response stored, confirmation email not sent. | PASS |
| TC-003 | Duplicate Lead | Duplicate lead should be detected and should not trigger another confirmation email. | Duplicate detected, workflow executed according to logic, no confirmation email sent. | PASS  |
| TC-004 | Missing Required Field | Form should prevent submission when required fields are blank. | Form displayed validation message and prevented submission. | PASS |

# Testing Summary

| Item | Result |
| ----- | :---- |
| Total Test Cases | 4 |
| Passed | 4 |
| Failed | 0 |
| Overall Status | Pass |

#  Conclusion

The Lead Capture & Validation Automation System was successfully tested using multiple scenarios, including valid lead submission, invalid email validation, duplicate lead detection, and required field validation. All executed test cases passed successfully. The automation workflow, Google Forms, Google Sheets, Gmail integration, and n8n workflow performed according to the implemented project requirements.

# Testing Evidence

Screenshots for all executed test cases have been saved in the project directory:

**Screenshots → Week 2 – Workflow Testing**

The evidence includes:

* Google Form submission   
* Google Sheets response   
* n8n workflow execution   
* Gmail confirmation email   
* Validation messages

