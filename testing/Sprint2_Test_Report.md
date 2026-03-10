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

**4. Booking**

To verify that students can start or book a tutoring session.

To ensure that the system properly handles session booking actions.

The purpose of these tests is to identify usability issues, system errors, and interface problems before the final implementation of the application.

## 2. Test Cases

| Test Case ID | Feature Tested | Test Scenario                                                | Expected Result                                                    | Result |
| ------------ | -------------- | ------------------------------------------------------------ | ------------------------------------------------------------------ | ------ |
| TC-01        | Login          | User enters valid email and password                         | User should successfully log in and be redirected to the dashboard | Pass   |
| TC-02        | Login          | User enters incorrect password                               | System should display an error message and prevent login           | Fail   |
| TC-03        | Search         | User searches for a subject such as "Algebra"                | Relevant course or tutor results should appear                     | Pass   |
| TC-04        | Booking        | User clicks the **Start** button to begin a learning session | Learning session should start successfully                         | Pass   |
| TC-05        | Quiz           | User answers the Algebra quiz question correctly             | System should mark the answer as correct                           | Fail   |

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

## Bug ID: MATH-001

**Bug Title:** Math Quiz Answer Validation Logic Error

**Description:**
During testing of the Algebra learning module, the system incorrectly evaluates answers in the quiz section. Even when a correct mathematical answer is entered, the system marks it as incorrect.

**Steps to Reproduce:**

1. Open the EduConnect prototype.
2. Navigate to the **Algebra 101** course.
3. Scroll to the **Quiz 1: Pre-test** section.
4. Click the **Start** button to begin the quiz.
5. Enter the correct answer to the math question.
6. Submit the answer.

**Expected Result:**
The system should correctly validate the answer and mark it as correct.

**Actual Result:**
The system incorrectly marks the correct answer as wrong.

**Severity Level:** High

