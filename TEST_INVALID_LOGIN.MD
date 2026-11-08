# Test Case 002: Login with Invalid Password

## Test Objective
Verify that the system blocks access and displays an appropriate error message when an incorrect password is entered.

## Pre-conditions
- User has an active registered account.
- User is on the login screen.

## Test Steps
1. Enter a registered email in the "Email" field.
2. Enter an incorrect or unregistered password in the "Password" field.
3. Click the "Login" button.

## Expected Result
- User remains on the login page (access is denied).
- Error message is displayed: "Invalid email or password."
