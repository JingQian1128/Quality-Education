1. **Test Objectives**

This testing process was aimed at testing the functionality and usability of the EduConnect mobile application prototype. The testing was aimed at ensuring that the main features of the system work properly and offer convenient user experience.

The primary characteristics that have been checked are:

1. **Registration**

To ensure that new users are able to create an account with ease.
To make sure that the necessary fields like email and password are obtained appropriately.

2. **Login**

To test the ability of the system to accept valid user credentials.
To confirm that the system responds to erroneous log-in information, correctly.

3. **Search**

To determine whether users are able to search the platform in tutor or learning resource.
In order to verify that the search functionality has found the right results.
The aim of these tests is to determine the problem in usability, system errors, and interface problem prior to the actual implementation of the application.

4. **Booking**

To ensure that students have the ability to start or to book a tutoring session.

To make sure that the system is able to deal with session booking actions.

These tests are used to find out the usability problems, system errors, and interface problems prior to the ultimate implementation of the application.

# 2. Test Cases**

Test Case ID	Feature tested	Test scenario	Expected result	Result
TC-01	Login	User is typing in valid email and password	User would be able to log in and take him or her to the dashboard successfully.
TC-02	Login	Wrong password is used by the user that should not be allowed to log in and system must show an error message.
TC-03	Search	The user types something like "Algebra" in the search box and relevant course/tutor should be found.
TC-04	Booking	User clicks Start button to open learning session	Learning session should open successfully Pass
TC-05	Quiz	User should get the answer to the question of Algebra quiz correct System should mark the answer as correct Failed.
# 3. Bug Reports

Bug ID: EC-001

Bug Title: Entry can be made with empty mandatory fields.

Description: In testing the registration feature, the system permitted users to use the registration form on occasions in which one left the necessary fields blank. This implies that the form validation is not a well implemented procedure.

Steps to Reproduce:

Launch EduConnect registration page.
Leave out one or more mandatory fields (e.g., email).
Click the Register button.
Result to Expect: This system ought to submit a form and a validation message should be given like this field is mandatory.

Real Life Result: The system enables the form to be submitted without any validation message being shown.

Severity Level: High

Bug ID: EC-002

Bug Title: No error message on use of wrong logins.

Description: In case the user attempts to log in with wrong credentials, the system fails to issue a relevant error message to make the user aware that the login attempt was unsuccessful.

Steps to Reproduce:

Click the EduConnect log in page.
Put in a registered email with an invalid password.
Click the Login button.
Predicted Outcome: An error message of the type should be shown on the system like: Incorrect email or password.

Real World Scenario: The user attempts to log in and nothing shows on the screen indicating an error.

Severity Level: Medium

Bug ID: MATH-001

Bug Name: Math Quiz Answer validation Logic Error.

Situation: When testing the Algebra learning module, the system was inaccurate in the evaluation of the answers in the quiz section. The system scans a correct mathematical answer and declares it to be incorrect even when the correct mathematical answer is typed in.

Steps to Reproduce:

Unzip EduConnect prototype.
Go into Algebra 101 course.
Click on the area Quiz 1: Pre-test.
When the quiz is started, you can press the Start button.
Write the correct math question answer.
Submit the answer.
Expected Result: The system would be able to validate the answer correctly and pose to mark the answer as correct.

Factual Findings: The system marks the correct answer wrong.

Severity Level: High

