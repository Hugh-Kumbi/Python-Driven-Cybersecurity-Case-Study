# Python-Driven-Cybersecurity-Case-Study

> This project, **"Python-Driven Cybersecurity Case Study,"** draws inspiration from the concepts presented in *Automate Cybersecurity Tasks with Python*. For further details and insights, please visit [link](https://www.coursera.org/learn/automate-cybersecurity-tasks-with-python) for further information.

## Automating Login Processes and Analyzing Patterns With Python

In this case study, I utilized Python to streamline the login process, perform an in-depth analysis of login data, and identify patterns using regular expressions. The project highlights how Python's automation capabilities can enhance cybersecurity workflows, improve efficiency, and uncover valuable insights from complex datasets.

### Scope and Objectives

This project presents three key scenarios that I developed and customized to demonstrate the practical application of Python in cybersecurity.

1. **Automating the Login Process:** Python is used to streamline and secure login operations.
2. **Analyzing Login Data:** Leveraging Python to gain insights and detect anomalies in login records.
3. **Identifying Patterns with Regular Expressions:** Using Python's regex capabilities to uncover and analyze patterns within the data.

The complete solutions and implementations are documented in the notebook titled **"Streamlined Security with Python Case Study.ipynb."**

### Scenario 1: Automating the Login Process

The security analyst team at ABC Association tasked me with automating their login process to reduce manual approval efforts. The goal was to develop a Python-based system that validates user credentials and device assignments automatically, ensuring a streamlined and secure authentication process.

**Task Overview**

The system needed to check the following conditions in sequence:

1. **User Validation:**

  * If the username matches the approved users list (case-sensitive), the system prints:
    *`<username> is approved.`*
  * If the username does not match, the system prints:
    *`<username> is not approved to access the system.`*
  * In this case, the system halts further checks for that username.

2. **Device Validation:**

  * If the username is approved, the system verifies the device ID.
  * If the device ID matches the assigned device for the user, the system prints: 
*`<device_id> is the assigned device for <username>.`*
  * If the device ID does not match, the system prints: 
*`<device_id> is not the assigned device for <username>.`*

**Input Details**
* **Approved Users and Devices List:**
  
| Users | Devices |
| :-: | :-: |
| vanessa | 245ahw |
| kevin | fkdjs238 |
| maria | 9hfks12 |
| keith | sdfhksd2 |

User 1: Device1
This information forms the basis for validating login attempts.

Implementation Notes
Python was chosen for its robust string manipulation and logical processing capabilities.
Special attention was given to ensure that username validation is case-sensitive.
This automated solution minimizes manual intervention while maintaining high security and accuracy in the authentication process.









