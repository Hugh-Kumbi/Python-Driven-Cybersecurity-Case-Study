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

## Scenario 3: Finding Patterns Using Regular Expressions

The security analyst team at XYZ Corp requested an investigation into patterns behind certain activities using Python. The goal was to leverage regular expressions to identify and analyze specific patterns in data, such as device IDs, malware signatures, and IP addresses.

### Task Overview

**The following activities were targeted for pattern identification:**

1. **Find the Hex Signature:** The malware signature `0x9ACDAB` needs to be extracted and analyzed from the provided data.
2. **Find Device IDs Starting with** `r15`: Extract and display device IDs that start with r15 from the list:

9x482kt
6oa6m6u
253be78
r15u9q5
ac742a1
x3463ac
g07h55q
41j1u2e
i4l56nq
r262c36
ii286fq
r151dm4
r15xk9h
1270t3o
2j33krk
081qc9t
zh86b2l
67bv8fy
r159r1u
42dr56i

3. **Find and Analyze IP Addresses:** Identify valid IP addresses in the form `192.xxx.xxx` from the following logs:

| Username | Current_day_logins |  Average_day_logins |
| :-: | :-: | :-: |
| daquino | 2024-11-08 7:02:35 | 192.168.168.144 |
| rjensen | 2024-11-20 0:59:26 | 192.168.213.128 |
| cjackson | 2025-01-05 19:36:42 | 192.168.247.153 |
| iuduike | 2024-11-15 6:46:40 | 192.168.22.115 |
| jrafael | 2024-12-01 22:40:01 | 192.168.148.115 |
| smartell | 2024-11-25 19:30:32 | 192.168.190.178 |
| asundara | 2024-12-10 18:38:07 | 192.168.96.200 |
| arutley | 2025-01-12 17:00:59 | 1923.1689.3.24 |
| dkot | 2024-12-20 10:52:00 | 1921.168.1283.75 |
| aestrada | 2024-11-30 19:28:12 | 1924.1680.27.57 |
| abernard | 2025-01-18 23:38:46 | 19245.168.2345.49 |
| alevitsk | 2024-11-05 12:09:10 | 192.16874.1390.176 |
| jclark | 2024-11-12 10:48:02 | 192.168.174.117 |
| eraab | 2024-11-22 6:03:41 | 192.168.152.148 |
| yappiah| 2025-01-09 10:37:22 | 192.168.103.10654 |

Using regular expressions, these tasks can be solved by identifying and extracting the necessary patterns. This approach will help automate the analysis of system logs and device activities.
