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

