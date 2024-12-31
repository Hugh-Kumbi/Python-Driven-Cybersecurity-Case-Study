# Automating Login Processes and Analyzing Patterns With Python

## Scenario 1: Automating the Login Process

The security analyst team at ABC Association tasked me with automating their login process to reduce manual approval efforts. The goal was to develop a Python-based system that validates user credentials and device assignments automatically, ensuring a streamlined and secure authentication process.

### Task Overview

**The system needed to check the following conditions in sequence:**

1. **User Validation:**

   * If the username matches the approved users list (case-sensitive), the system prints: <br />
    *`<username> is approved.`*
   * If the username does not match, the system prints: <br />
    *`<username> is not approved to access the system.`*
   * In this case, the system halts further checks for that username.

2. **Device Validation:**

   * If the username is approved, the system verifies the device ID.
   * If the device ID matches the assigned device for the user, the system prints: <br />
*`<device_id> is the assigned device for <username>.`*
   * If the device ID does not match, the system prints: <br />
*`<device_id> is not the assigned device for <username>.`*

### Input Details
* **Approved Users and Devices List:**
  
| Users | Devices |
| :-: | :-: |
| vanessa | 245ahw |
| kevin | fkdjs238 |
| maria | 9hfks12 |
| keith | sdfhksd2 |

This information forms the basis for validating login attempts.

### Implementation Notes

  * Python was chosen for its robust string manipulation and logical processing capabilities.
  * Special attention was given to ensure that username validation is case-sensitive.

This automated solution minimizes manual intervention while maintaining high security and accuracy in the authentication process.

## Scenario 2: Analyzing Login Activities

The security analyst team at ABC Association has asked me to analyze login activities based on conditional statements using Python. The goal was to automate the process of analyzing login data to provide valuable insights, including the total logins for the current day, the average logins per day for a user, and issuing an alert if the login activity exceeds normal levels.

### Task Overview
**The system needed to address the following key objectives:**

1. **Total Login Count for Current Day:** Display the total number of logins for the current day.
2. **Average Logins Per Day:** Calculate and display the average number of logins per day for the user.
3. **Alert for Excessive Login Activity:** If the login ratio (current day logins divided by average day logins) exceeds a threshold of 3, the system should trigger an alert.

For example, if the **current day logins** is 2 and the **average day logins** is 1, the **login ratio** will be 2/1 = 2, which is not high enough to trigger an alert. However, if the **current day logins** is 4, the login ratio would be 4/1 = 4, triggering an alert.

### Input Details

* **User Data:**

| Username | Current_day_logins |  Average_day_logins |
| :-: | :-: | :-: |
| vanessa | 10 | 5 |
| kevin | 8 | 6 |
| maria | 4 | 1 |
| keith | 7 | 3 |

### Approach

* **Model 1:** Basic solution using conditional statements and simple calculations.
* **Model 1 Widget:** Incorporating an interactive widget for better user interaction and real-time display of results.
* **Model 2:** A more advanced solution with additional features for scalability or flexibility.
* **Model 2 Widget:** Enhanced widget implementation for a more user-friendly and dynamic analysis experience.

This analysis helps detect abnormal login activity, providing the security team with the necessary information to investigate potential security threats.









