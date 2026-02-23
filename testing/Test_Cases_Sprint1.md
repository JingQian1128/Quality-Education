
# Test Cases - Sprint 1  


---
1. Registration  

| Test ID | Test Scenario | Expected Result | Actual Result | Status |
|---------|--------------|----------------|--------------|--------|
| TC-REG-01 | Register with valid name, email and strong password | Account is created successfully. A success message is displayed and user is redirected to the login/dashboard page. |  |  |
| TC-REG-02 | Register with blank email field | System does not allow submission and displays validation message: "Email is required." |  |  |
| TC-REG-03 | Register with invalid email address (e.g., abc@com) | System displays error message "Please enter a valid email address" and prevents registration. |  |  |
| TC-REG-04 | Register using weak password (less than required length) | System does not allow registration and shows password requirement message. |  |  |
| TC-REG-05 | Register with an already registered email | System displays error "Email exists" and does not allow creation of duplicate account. |  |  |

---

 2. Login  

| Test ID | Test Scenario | Expected Result | Actual Result | Status |
|---------|--------------|----------------|--------------|--------|
| TC-LOG-01 | Log in using registered email and correct password | User is successfully logged in and redirected to the Dashboard page. |  |  |
| TC-LOG-02 | Log in using wrong password | Login fails and error message "Incorrect email or password" is displayed. |  |  |
| TC-LOG-03 | Log in using unregistered email | System shows error message stating that no account exists. |  |  |
| TC-LOG-04 | Log in using empty email and password fields | System does not allow login and displays required field validation messages. |  |  |
| TC-LOG-05 | Logout after successful login | User is logged out successfully and redirected to the Login page. |  |  |

---

3. Browse & Search Tutors  

| Test ID | Test Scenario | Expected Result | Actual Result | Status |
|---------|--------------|----------------|--------------|--------|
| TC-SR-01 | Search for a subject that exists (e.g., Mathematics) | System lists relevant tutors for the selected subject. |  |  |
| TC-SR-02 | Search for a subject with no tutors available | System displays "No results found" message clearly. |  |  |
| TC-SR-03 | Search using partial keyword (e.g., Math) | System displays tutor results matching the keyword entered. |  |  |
| TC-SR-04 | Search with empty search field | System asks the user to enter a subject or displays all tutors (based on system design). |  |  |
| TC-SR-05 | Apply subject filter and additional filter (e.g., price range) | Results update correctly based on selected filters. |  |  |

---

 Notes  

- During system testing, **Actual Result** and **Status** will be updated.  
- All failed test cases will be reported as bugs in the project repository.
