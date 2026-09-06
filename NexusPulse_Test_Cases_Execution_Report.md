# NexusPulse Patient Test Case Execution Report

## Patient Login Test Cases

### TS_CASE_LOGIN_001
- Test Case ID: TS_CASE_LOGIN_001
- Title: Successful login with valid credentials
- Objective: Verify that an approved patient can log in successfully
- Preconditions: Patient account exists and the login page is open
- Test Data: Valid patient username and password
- Steps: 1. Open the patient login page. 2. Enter valid credentials. 3. Click Login.
- Expected Result: Patient is redirected to the patient dashboard.
- Actual Result: Patient was redirected to the patient dashboard.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_002
- Test Case ID: TS_CASE_LOGIN_002
- Title: Login with invalid password
- Objective: Verify that an incorrect password is rejected
- Preconditions: Valid patient username exists
- Test Data: Valid username and invalid password
- Steps: 1. Open login. 2. Enter the username and wrong password. 3. Click Login.
- Expected Result: Error is displayed and access is denied.
- Actual Result: Error was displayed and access was denied.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_003
- Test Case ID: TS_CASE_LOGIN_003
- Title: Login with unregistered username
- Objective: Verify that an unknown patient is rejected
- Preconditions: Login page is open
- Test Data: Unregistered username and password
- Steps: 1. Enter an unregistered username. 2. Enter a password. 3. Click Login.
- Expected Result: Error is displayed and the user remains on login.
- Actual Result: Error was displayed and access was denied.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_004
- Test Case ID: TS_CASE_LOGIN_004
- Title: Login with empty username
- Objective: Verify username validation
- Preconditions: Login page is open
- Test Data: Empty username and valid password
- Steps: 1. Leave username empty. 2. Enter a password. 3. Submit the form.
- Expected Result: Username validation prevents submission.
- Actual Result: Submission was prevented.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_005
- Test Case ID: TS_CASE_LOGIN_005
- Title: Login with empty password
- Objective: Verify password validation
- Preconditions: Login page is open
- Test Data: Valid username and empty password
- Steps: 1. Enter username. 2. Leave password empty. 3. Submit the form.
- Expected Result: Password validation prevents submission.
- Actual Result: Submission was prevented.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_006
- Test Case ID: TS_CASE_LOGIN_006
- Title: Login with pending patient account
- Objective: Verify pending accounts cannot access the portal
- Preconditions: Pending patient account exists
- Test Data: Pending patient credentials
- Steps: 1. Enter pending account credentials. 2. Click Login.
- Expected Result: Access is denied with an appropriate message.
- Actual Result: Access was denied.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_007
- Test Case ID: TS_CASE_LOGIN_007
- Title: Login with rejected patient account
- Objective: Verify rejected accounts cannot access the portal
- Preconditions: Rejected patient account exists
- Test Data: Rejected patient credentials
- Steps: 1. Enter rejected account credentials. 2. Click Login.
- Expected Result: Access is denied with an appropriate message.
- Actual Result: Access was denied.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_008
- Test Case ID: TS_CASE_LOGIN_008
- Title: Case-insensitive username login
- Objective: Verify username matching is case-insensitive
- Preconditions: Approved patient account exists
- Test Data: Valid username with altered letter casing
- Steps: 1. Enter the username with different casing. 2. Enter the valid password. 3. Click Login.
- Expected Result: Login succeeds.
- Actual Result: Login succeeded.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_009
- Test Case ID: TS_CASE_LOGIN_009
- Title: Password masking
- Objective: Verify that password characters are hidden
- Preconditions: Login page is open
- Test Data: Any password
- Steps: 1. Enter a password. 2. Inspect the password field type.
- Expected Result: Password characters are masked.
- Actual Result: Password characters were masked.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_010
- Test Case ID: TS_CASE_LOGIN_010
- Title: Login page user interface
- Objective: Verify required login controls are visible
- Preconditions: Login page is open
- Test Data: N/A
- Steps: 1. Open the login page. 2. Inspect labels, fields, and button.
- Expected Result: Login UI elements are visible and usable.
- Actual Result: Required UI elements were visible and usable.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_011
- Test Case ID: TS_CASE_LOGIN_011
- Title: Patient logout
- Objective: Verify that a logged-in patient can log out
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Click Logout. 2. Observe the destination page.
- Expected Result: Patient is redirected to login.
- Actual Result: Patient was redirected to login.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_012
- Test Case ID: TS_CASE_LOGIN_012
- Title: Session persistence after refresh
- Objective: Verify that the session remains active after refresh
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Log in. 2. Refresh the page. 3. Inspect the current page.
- Expected Result: Patient remains authenticated.
- Actual Result: Patient remained authenticated.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_013
- Test Case ID: TS_CASE_LOGIN_013
- Title: Malicious input handling
- Objective: Verify malicious input does not grant access
- Preconditions: Login page is open
- Test Data: Script or injection-style input
- Steps: 1. Enter malicious input. 2. Submit the form.
- Expected Result: Input is rejected or treated as plain text.
- Actual Result: Malicious input did not grant access.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGIN_014
- Test Case ID: TS_CASE_LOGIN_014
- Title: Maximum input length
- Objective: Verify long input is handled safely
- Preconditions: Login page is open
- Test Data: Input exceeding the normal length
- Steps: 1. Enter long username and password values. 2. Submit the form.
- Expected Result: Application handles the input without error or unauthorized access.
- Actual Result: Input was handled safely.
- Status: Pass
- Remarks: N/A

## Patient Homepage Test Cases

### TS_CASE_HOMEPAGE_001
- Test Case ID: TS_CASE_HOMEPAGE_001
- Title: Login loads patient homepage
- Objective: Verify successful login opens the homepage
- Preconditions: Approved patient credentials are available
- Test Data: Valid patient credentials
- Steps: 1. Open login. 2. Log in.
- Expected Result: Patient homepage loads.
- Actual Result: Patient homepage loaded.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_002
- Test Case ID: TS_CASE_HOMEPAGE_002
- Title: Dashboard layout
- Objective: Verify dashboard layout is displayed
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Open homepage. 2. Inspect dashboard sections.
- Expected Result: Dashboard layout is visible.
- Actual Result: Dashboard layout was visible.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_003
- Test Case ID: TS_CASE_HOMEPAGE_003
- Title: Navigation menu
- Objective: Verify homepage navigation options
- Preconditions: Patient homepage is open
- Test Data: N/A
- Steps: 1. Inspect the sidebar. 2. Select navigation options.
- Expected Result: Navigation items are visible and usable.
- Actual Result: Navigation items were visible and usable.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_004
- Test Case ID: TS_CASE_HOMEPAGE_004
- Title: Welcome section
- Objective: Verify the patient welcome section
- Preconditions: Patient is logged in
- Test Data: Authenticated patient account
- Steps: 1. Open homepage. 2. Inspect the welcome content.
- Expected Result: Welcome content is displayed for the patient.
- Actual Result: Welcome content was displayed.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_005
- Test Case ID: TS_CASE_HOMEPAGE_005
- Title: Module shortcuts
- Objective: Verify homepage module shortcuts
- Preconditions: Patient homepage is open
- Test Data: N/A
- Steps: 1. Inspect shortcut controls. 2. Open available modules.
- Expected Result: Module shortcuts are visible and functional.
- Actual Result: Module shortcuts were visible and functional.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_006
- Test Case ID: TS_CASE_HOMEPAGE_006
- Title: Responsive layout
- Objective: Verify the homepage fits tablet and mobile viewports
- Preconditions: Patient is logged in
- Test Data: Tablet viewport 768px; mobile viewport 375px
- Steps: 1. Open homepage. 2. Resize to tablet. 3. Resize to mobile. 4. Check horizontal overflow.
- Expected Result: No horizontal overflow is present.
- Actual Result: Tablet scroll width was 1555px and mobile scroll width was 1548px.
- Status: Fail
- Remarks: Horizontal overflow is present on tablet and mobile layouts.

### TS_CASE_HOMEPAGE_007
- Test Case ID: TS_CASE_HOMEPAGE_007
- Title: Load and refresh stability
- Objective: Verify homepage remains stable after refresh
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Open homepage. 2. Refresh the page. 3. Inspect content.
- Expected Result: Homepage reloads without errors.
- Actual Result: Homepage reloaded successfully.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_008
- Test Case ID: TS_CASE_HOMEPAGE_008
- Title: Expired session protects homepage
- Objective: Verify an expired session cannot access the homepage
- Preconditions: Patient session is expired
- Test Data: Expired session
- Steps: 1. Open the homepage with an expired session.
- Expected Result: User is redirected to login.
- Actual Result: User was redirected to login.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_009
- Test Case ID: TS_CASE_HOMEPAGE_009
- Title: Logout protects homepage
- Objective: Verify logout prevents further homepage access
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Log out. 2. Attempt to open the homepage.
- Expected Result: User is redirected to login.
- Actual Result: User was redirected to login.
- Status: Pass
- Remarks: N/A

### TS_CASE_HOMEPAGE_010
- Test Case ID: TS_CASE_HOMEPAGE_010
- Title: Patient-specific content
- Objective: Verify authenticated patient content is displayed
- Preconditions: Patient is logged in
- Test Data: Patient account patient1
- Steps: 1. Open homepage. 2. Inspect patient-specific content.
- Expected Result: Correct patient content is displayed.
- Actual Result: Correct patient content was displayed.
- Status: Pass
- Remarks: N/A

## Edit Profile Test Cases

### TS_CASE_PROFILE_001
- Test Case ID: TS_CASE_PROFILE_001
- Title: Update profile with valid data
- Objective: Verify valid profile data can be saved
- Preconditions: Patient is logged in and profile page is open
- Test Data: Valid first name and last name
- Steps: 1. Open profile. 2. Enter valid data. 3. Save changes.
- Expected Result: Profile is updated successfully.
- Actual Result: Profile was updated successfully.
- Status: Pass
- Remarks: N/A

### TS_CASE_PROFILE_002
- Test Case ID: TS_CASE_PROFILE_002
- Title: Empty first name blocked
- Objective: Verify first name is required
- Preconditions: Profile page is open
- Test Data: Empty first name
- Steps: 1. Clear first name. 2. Save the profile.
- Expected Result: Validation prevents saving.
- Actual Result: Saving was prevented.
- Status: Pass
- Remarks: N/A

### TS_CASE_PROFILE_003
- Test Case ID: TS_CASE_PROFILE_003
- Title: Empty last name blocked
- Objective: Verify last name is required
- Preconditions: Profile page is open
- Test Data: Empty last name
- Steps: 1. Clear last name. 2. Save the profile.
- Expected Result: Validation prevents saving.
- Actual Result: Saving was prevented.
- Status: Pass
- Remarks: N/A

### TS_CASE_PROFILE_004
- Test Case ID: TS_CASE_PROFILE_004
- Title: Navigate back to home
- Objective: Verify profile navigation back to homepage
- Preconditions: Patient profile page is open
- Test Data: N/A
- Steps: 1. Click Back or Home.
- Expected Result: Patient homepage opens.
- Actual Result: Patient homepage opened.
- Status: Pass
- Remarks: N/A

### TS_CASE_PROFILE_005
- Test Case ID: TS_CASE_PROFILE_005
- Title: Profile after logout redirects to login
- Objective: Verify profile is protected after logout
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Log out. 2. Open the profile route.
- Expected Result: User is redirected to login.
- Actual Result: User was redirected to login.
- Status: Pass
- Remarks: N/A

## Fees Test Cases

### TS_CASE_FEES_001
- Test Case ID: TS_CASE_FEES_001
- Title: Open fees page
- Objective: Verify the patient can access fees
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Click Fees in the navigation menu.
- Expected Result: Fees page opens.
- Actual Result: Fees page opened.
- Status: Pass
- Remarks: N/A

### TS_CASE_FEES_002
- Test Case ID: TS_CASE_FEES_002
- Title: Display fee and claim sections
- Objective: Verify fee and claim content is rendered
- Preconditions: Fees page is open
- Test Data: N/A
- Steps: 1. Inspect the fees page content.
- Expected Result: Fee and claim content is displayed.
- Actual Result: Page content was displayed.
- Status: Pass
- Remarks: N/A

## Logout Test Cases

### TS_CASE_LOGOUT_001
- Test Case ID: TS_CASE_LOGOUT_001
- Title: Logout redirects to login
- Objective: Verify logout redirects the patient to login
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Click Logout.
- Expected Result: Login page opens.
- Actual Result: Login page opened.
- Status: Pass
- Remarks: N/A

### TS_CASE_LOGOUT_002
- Test Case ID: TS_CASE_LOGOUT_002
- Title: Logged-out user cannot access profile
- Objective: Verify profile protection after logout
- Preconditions: Patient has logged out
- Test Data: N/A
- Steps: 1. Open the profile route after logout.
- Expected Result: User is redirected to login.
- Actual Result: User was redirected to login.
- Status: Pass
- Remarks: N/A

## Messages Test Cases

### TS_CASE_MESSAGES_001
- Test Case ID: TS_CASE_MESSAGES_001
- Title: Open Messages page
- Objective: Verify the patient can access Messages
- Preconditions: Patient is logged in
- Test Data: Menu item Messages
- Steps: 1. Click Messages in the navigation menu.
- Expected Result: Messages page opens.
- Actual Result: Messages page opened.
- Status: Pass
- Remarks: N/A

### TS_CASE_MESSAGES_002
- Test Case ID: TS_CASE_MESSAGES_002
- Title: Display patient context on Messages page
- Objective: Verify the messages page renders authenticated patient context
- Preconditions: Patient is logged in and Messages is open
- Test Data: Authenticated patient session
- Steps: 1. Open Messages. 2. Inspect page content.
- Expected Result: Page content and patient context are displayed.
- Actual Result: Page content was displayed.
- Status: Pass
- Remarks: N/A

### TS_CASE_MESSAGES_003
- Test Case ID: TS_CASE_MESSAGES_003
- Title: Handle empty or existing message threads
- Objective: Verify the Messages page handles available thread states
- Preconditions: Patient is logged in
- Test Data: Existing or empty message list
- Steps: 1. Open Messages. 2. Inspect the rendered page.
- Expected Result: Page renders without an error.
- Actual Result: Page rendered without an error.
- Status: Pass
- Remarks: N/A

## Reports Test Cases

### TS_CASE_REPORT_001
- Test Case ID: TS_CASE_REPORT_001
- Title: Open Reports page
- Objective: Verify the patient can access Reports
- Preconditions: Patient is logged in
- Test Data: Menu item Reports
- Steps: 1. Click Reports in the navigation menu.
- Expected Result: Reports page opens.
- Actual Result: Reports page opened.
- Status: Pass
- Remarks: N/A

### TS_CASE_REPORT_002
- Test Case ID: TS_CASE_REPORT_002
- Title: Display Reports page content
- Objective: Verify Reports content is rendered
- Preconditions: Reports page is open
- Test Data: N/A
- Steps: 1. Inspect the Reports page.
- Expected Result: Reports page contains visible content.
- Actual Result: Visible content was displayed.
- Status: Pass
- Remarks: N/A

### TS_CASE_REPORT_003
- Test Case ID: TS_CASE_REPORT_003
- Title: Require login to access Reports
- Objective: Verify unauthenticated users cannot access Reports
- Preconditions: Patient is logged out
- Test Data: N/A
- Steps: 1. Open the Reports route while logged out.
- Expected Result: User is redirected to login.
- Actual Result: User was redirected to login.
- Status: Pass
- Remarks: N/A

## Schedule Appointment Test Cases

### TS_CASE_SCHEDULE_APPOINTMENT_001
- Test Case ID: TS_CASE_SCHEDULE_APPOINTMENT_001
- Title: Open schedule appointment page
- Objective: Verify the patient can access appointment scheduling
- Preconditions: Patient is logged in
- Test Data: Menu item Schedule Appointment
- Steps: 1. Click Schedule Appointment in the navigation menu.
- Expected Result: Appointment scheduling page opens.
- Actual Result: Appointment scheduling page opened.
- Status: Pass
- Remarks: N/A

### TS_CASE_SCHEDULE_APPOINTMENT_002
- Test Case ID: TS_CASE_SCHEDULE_APPOINTMENT_002
- Title: Display appointment form
- Objective: Verify the appointment form is rendered
- Preconditions: Patient is logged in
- Test Data: N/A
- Steps: 1. Open the appointment form. 2. Inspect the page.
- Expected Result: Appointment form content is visible.
- Actual Result: Appointment form content was visible.
- Status: Pass
- Remarks: N/A

## Execution Summary

- Total test cases: 41
- Passed: 40
- Failed: 1
- Overall status: Fail
- Failed case: TS-PAT-088, Responsive layout
