# Automating Login Processes and Analyzing Patterns With Python

### Scenario 1: Automating the Login Process

The security analyst team at ABC Association tasked me with automating their login process to reduce manual approval efforts. The goal was to develop a Python-based system that validates user credentials and device assignments automatically, ensuring a streamlined and secure authentication process.

**Task Overview**

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

**Input Details**
* **Approved Users and Devices List:**
  
| Users | Devices |
| :-: | :-: |
| vanessa | 245ahw |
| kevin | fkdjs238 |
| maria | 9hfks12 |
| keith | sdfhksd2 |

This information forms the basis for validating login attempts.

**Implementation Notes**

  * Python was chosen for its robust string manipulation and logical processing capabilities.
  * Special attention was given to ensure that username validation is case-sensitive.

This automated solution minimizes manual intervention while maintaining high security and accuracy in the authentication process.
