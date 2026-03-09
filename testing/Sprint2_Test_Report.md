# 1. Test Objectives

The objective of this testing process was to evaluate the functionality and usability of the EduConnect mobile application prototype. The testing focused on verifying whether the core features of the system operate correctly and provide a smooth user experience.

The main features tested include:

**1. Registration**

* To verify that new users can create an account successfully.
* To ensure that required fields such as email and password are properly captured.

**2. Login**

* To check whether existing users can log into the system using valid credentials.
* To verify that the system handles incorrect login details appropriately.

**3. Search**

* To test whether users can search for tutors or learning resources within the platform.
* To confirm that the search function returns relevant results.

The purpose of these tests is to identify usability issues, system errors, and interface problems before the final implementation of the application.
# 2. Test Results

| Test Case ID | Feature Tested     | Test Scenario                                               | Expected Result                          | Result |
| ------------ | ------------------ | ----------------------------------------------------------- | ---------------------------------------- | ------ |
| TC-01        | Registration       | User enters valid registration details and submits the form | Account should be created successfully   | Pass   |
| TC-02        | Registration       | User submits form with empty required fields                | System should display validation message | Fail   |
| TC-04        | Login              | User enters incorrect login credentials                     | System should display error message      | Fail   |
| TC-05        | Identity Selection | User selects Student identity                               | Student option should be highlighted     | Pass   |
| TC-06        | Search             | User searches for a tutor                                   | Relevant tutor results should appear     | Pass   |
# # 3. Bug Reports

## Bug ID: EC-001

**Bug Title:** Registration allows submission with empty required fields

**Description:**
During testing of the registration feature, the system allowed users to submit the registration form even when required fields were left empty. This indicates that the form validation is not properly enforced.

**Steps to Reproduce:**

1. Open the EduConnect registration page.
2. Leave one or more required fields (e.g., email) empty.
3. Click the **Register** button.

**Expected Result:**
The system should prevent form submission and display a validation message such as **“This field is required.”**

**Actual Result:**
The system allows the form to be submitted without displaying any validation message.

**Severity Level:** High

---

## Bug ID: EC-002

**Bug Title:** No error message displayed for incorrect login credentials

**Description:**
When users attempt to log in using incorrect credentials, the system does not display an appropriate error message to inform the user that the login attempt failed.

**Steps to Reproduce:**

1. Open the EduConnect login page.
2. Enter a registered email with an incorrect password.
3. Click the **Login** button.

**Expected Result:**
The system should display an error message such as **“Incorrect email or password.”**

**Actual Result:**
The login attempt fails but no clear error message is displayed to the user.

**Severity Level:** Medium
