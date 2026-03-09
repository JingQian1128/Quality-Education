1. Registration
   
| Test ID   | Test Scenario                                            | Expected Result                                                                                                     | Actual Result                                                                  | Status |
| --------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ------ |
| TC-REG-01 | Register with valid name, email and strong password      | Account is created successfully. A success message is displayed and user is redirected to the login/dashboard page. | Registration completed successfully and user was redirected to login page.     | Pass   |
| TC-REG-02 | Register with blank email field                          | System does not allow submission and displays validation message: "Email is required."                              | System prevented registration and displayed required field validation message. | Pass   |
| TC-REG-03 | Register with invalid email address (e.g., abc@com)      | System displays error message "Please enter a valid email address" and prevents registration.                       | System allowed submission without proper validation.                           | Fail   |
| TC-REG-04 | Register using weak password (less than required length) | System does not allow registration and shows password requirement message.                                          | System did not properly validate password strength.                            | Fail   |
| TC-REG-05 | Register with an already registered email                | System displays error "Email exists" and does not allow creation of duplicate account.                              | System displayed error message preventing duplicate account.| Pass   |

2. Login

 | Test ID   | Test Scenario                                      | Expected Result                                                              | Actual Result                                                | Status |
| --------- | -------------------------------------------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------------ | ------ |
| TC-LOG-01 | Log in using registered email and correct password | User is successfully logged in and redirected to the Dashboard page.         | Login successful and user redirected to dashboard.           | Pass   |
| TC-LOG-02 | Log in using wrong password                        | Login fails and error message "Incorrect email or password" is displayed.    | System displayed error message and prevented login.          | Pass   |
| TC-LOG-03 | Log in using unregistered email                    | System shows error message stating that no account exists.                   | System displayed account not found message.                  | Pass   |
| TC-LOG-04 | Log in using empty email and password fields       | System does not allow login and displays required field validation messages. | Login button remained active without validation message.     | Fail   |
| TC-LOG-05 | Logout after successful login                      | User is logged out successfully and redirected to the Login page.            | Logout function worked correctly and returned to login page. | Pass   |

3. Browse & Search Tutors

   | Test ID  | Test Scenario                                                  | Expected Result                                                                          | Actual Result                                        | Status |
| -------- | -------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------- | ------ |
| TC-SR-01 | Search for a subject that exists (e.g., Mathematics)           | System lists relevant tutors for the selected subject.                                   | Relevant tutors were displayed in the results list.  | Pass   |
| TC-SR-02 | Search for a subject with no tutors available                  | System displays "No results found" message clearly.                                      | System displayed "No tutors available" message.      | Pass   |
| TC-SR-03 | Search using partial keyword (e.g., Math)                      | System displays tutor results matching the keyword entered.                              | Partial keyword search returned matching tutors.     | Pass   |
| TC-SR-04 | Search with empty search field                                 | System asks the user to enter a subject or displays all tutors (based on system design). | System displayed all available tutors.               | Pass   |
| TC-SR-05 | Apply subject filter and additional filter (e.g., price range) | Results update correctly based on selected filters.                                      | Filter applied but results did not update correctly. | Fail   |
