# NexusPulse Patient Test Cases

| Test Case ID | Title | Objective | Preconditions | Test Data | Steps | Expected Result | Actual Result | Status | Remarks |
|---|---|---|---|---|---|---|---|---|---|
| TS_CASE_LOGIN_001 | Successful login with valid credentials | Verify approved patient login | Approved account; login page open | Valid credentials | Enter credentials; click Login | Dashboard opens | Dashboard opened | Pass | N/A |
| TS_CASE_LOGIN_002 | Login with invalid password | Reject incorrect password | Valid account exists | Wrong password | Enter credentials; click Login | Error displayed; access denied | Error displayed; access denied | Pass | N/A |
| TS_CASE_LOGIN_003 | Login with unregistered username | Reject unknown patient | Login page open | Unknown username | Enter credentials; click Login | Error displayed; access denied | Error displayed; access denied | Pass | N/A |
| TS_CASE_LOGIN_004 | Login with empty username | Validate required username | Login page open | Empty username | Submit empty username | Validation prevents submission | Submission prevented | Pass | N/A |
| TS_CASE_LOGIN_005 | Login with empty password | Validate required password | Login page open | Empty password | Submit empty password | Validation prevents submission | Submission prevented | Pass | N/A |
| TS_CASE_LOGIN_006 | Login with pending patient account | Reject pending account | Pending account exists | Pending credentials | Submit credentials | Access denied | Access denied | Pass | N/A |
| TS_CASE_LOGIN_007 | Login with rejected patient account | Reject rejected account | Rejected account exists | Rejected credentials | Submit credentials | Access denied | Access denied | Pass | N/A |
| TS_CASE_LOGIN_008 | Case-insensitive username login | Verify username casing | Approved account exists | Altered username case | Login with altered case | Login succeeds | Login succeeded | Pass | N/A |
| TS_CASE_LOGIN_009 | Password masking | Hide password characters | Login page open | Any password | Enter password | Characters are masked | Characters were masked | Pass | N/A |
| TS_CASE_LOGIN_010 | Login page UI | Verify login controls | Login page open | N/A | Inspect login controls | Controls are visible and usable | Controls were visible and usable | Pass | N/A |
| TS_CASE_LOGIN_011 | Patient logout | Verify patient logout | Patient logged in | N/A | Click Logout | Login page opens | Login page opened | Pass | N/A |
| TS_CASE_LOGIN_012 | Session persistence after refresh | Verify session remains active | Patient logged in | N/A | Refresh page | Patient remains authenticated | Patient remained authenticated | Pass | N/A |
| TS_CASE_LOGIN_013 | Malicious input handling | Verify unsafe input is rejected | Login page open | Injection-style input | Submit malicious input | No unauthorized access | No unauthorized access granted | Pass | N/A |
| TS_CASE_LOGIN_014 | Maximum input length | Verify long input is handled safely | Login page open | Long username and password | Submit long values | No error or unauthorized access | Input handled safely | Pass | N/A |
| TS_CASE_HOMEPAGE_083 | Login loads patient homepage | Verify homepage opens after login | Valid credentials available | Valid credentials | Login to portal | Homepage loads | Homepage loaded | Pass | N/A |
| TS_CASE_HOMEPAGE_084 | Dashboard layout | Verify dashboard layout | Patient logged in | N/A | Inspect dashboard | Layout is visible | Layout was visible | Pass | N/A |
| TS_CASE_HOMEPAGE_085 | Navigation menu | Verify navigation options | Homepage open | N/A | Inspect sidebar and links | Navigation items are usable | Navigation items were usable | Pass | N/A |
| TS_CASE_HOMEPAGE_086 | Welcome section | Verify welcome content | Patient logged in | Patient account | Inspect welcome area | Patient welcome is displayed | Welcome was displayed | Pass | N/A |
| TS_CASE_HOMEPAGE_087 | Module shortcuts | Verify module shortcuts | Homepage open | Module links | Open shortcuts | Shortcuts navigate correctly | Shortcuts worked | Pass | N/A |
| TS_CASE_HOMEPAGE_088 | Responsive layout | Verify tablet and mobile layout | Patient logged in | 768px and 375px viewports | Resize page; check overflow | No horizontal overflow | Tablet width 1555px; mobile width 1548px | Fail | Responsive overflow detected |
| TS_CASE_HOMEPAGE_089 | Load and refresh stability | Verify refresh stability | Patient logged in | N/A | Refresh homepage | Homepage reloads without errors | Homepage reloaded successfully | Pass | N/A |
| TS_CASE_HOMEPAGE_090 | Expired session protection | Protect homepage after expiry | Session expired | Expired session | Open homepage | Redirect to login | Redirected to login | Pass | N/A |
| TS_CASE_HOMEPAGE_091 | Logout homepage protection | Protect homepage after logout | Patient logged in | N/A | Logout; open homepage | Redirect to login | Redirected to login | Pass | N/A |
| TS_CASE_HOMEPAGE_092 | Patient-specific content | Verify correct patient information | Patient logged in | patient1 | Inspect homepage | Correct patient content appears | Correct patient content appeared | Pass | N/A |
| TS_CASE_PROFILE_051 | Update profile with valid data | Verify valid profile update | Profile page open | Valid first and last names | Edit and save profile | Profile is updated | Profile was updated | Pass | N/A |
| TS_CASE_PROFILE_053 | Empty first name blocked | Verify first name validation | Profile page open | Empty first name | Clear first name; save | Save is blocked | Save was blocked | Pass | N/A |
| TS_CASE_PROFILE_054 | Empty last name blocked | Verify last name validation | Profile page open | Empty last name | Clear last name; save | Save is blocked | Save was blocked | Pass | N/A |
| TS_CASE_PROFILE_059 | Navigate back to home | Verify profile navigation | Profile page open | N/A | Click Back/Home | Homepage opens | Homepage opened | Pass | N/A |
| TS_CASE_PROFILE_062 | Profile after logout redirects to login | Verify profile protection | Patient logged in | N/A | Logout; open profile | Redirect to login | Redirected to login | Pass | N/A |
| TS_CASE_FEES_015 | Open fees page | Verify fees access | Patient logged in | N/A | Click Fees | Fees page opens | Fees page opened | Pass | N/A |
| TS_CASE_FEES_016 | Display fee and claim sections | Verify fee content | Fees page open | N/A | Inspect fees page | Fee and claim content appears | Content appeared | Pass | N/A |
| TS_CASE_LOGOUT_001 | Logout redirects to login | Verify logout destination | Patient logged in | N/A | Click Logout | Login page opens | Login page opened | Pass | N/A |
| TS_CASE_LOGOUT_002 | Logged-out user cannot access profile | Verify profile protection | Patient logged out | N/A | Open profile route | Redirect to login | Redirected to login | Pass | N/A |
| TS_CASE_MESSAGES_073 | Open Messages page | Verify Messages access | Patient logged in | Messages menu | Click Messages | Messages page opens | Messages page opened | Pass | N/A |
| TS_CASE_MESSAGES_074 | Display patient context on Messages page | Verify authenticated patient context | Messages page open | Authenticated session | Inspect page | Patient context is displayed | Page content displayed | Pass | N/A |
| TS_CASE_MESSAGES_075 | Handle empty or existing message threads | Verify thread-state handling | Patient logged in | Existing or empty threads | Open Messages | Page renders without error | Page rendered without error | Pass | N/A |
| TS_CASE_REPORT_063 | Open Reports page | Verify Reports access | Patient logged in | Reports menu | Click Reports | Reports page opens | Reports page opened | Pass | N/A |
| TS_CASE_REPORT_064 | Display Reports page content | Verify report content | Reports page open | N/A | Inspect Reports page | Content is displayed | Content was displayed | Pass | N/A |
| TS_CASE_REPORT_065 | Require login to access Reports | Verify Reports authorization | Patient logged out | N/A | Open Reports route | Redirect to login | Redirected to login | Pass | N/A |
| TS_CASE_SCHEDULE_APPOINTMENT_029 | Open schedule appointment page | Verify scheduling access | Patient logged in | Appointment menu | Click Schedule Appointment | Scheduling page opens | Scheduling page opened | Pass | N/A |
| TS_CASE_SCHEDULE_APPOINTMENT_030 | Display appointment form | Verify appointment form | Appointment page open | N/A | Inspect appointment page | Form is visible | Form was visible | Pass | N/A |

**Execution summary:** 41 test cases, 40 passed, 1 failed. The failed case is `TS_CASE_HOMEPAGE_088` due to horizontal overflow on tablet and mobile viewports.
