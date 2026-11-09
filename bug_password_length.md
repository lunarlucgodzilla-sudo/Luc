# Bug Report: BUG-002 - Sign-up page accepts passwords shorter than 8 characters

## Metadata
- **Reporter:** Luc
- **Environment:** Chrome / Windows 11 / ThinkPad T14 / Staging
- **Date:** 2026-11-09
- **Severity / Priority:** Medium / Medium

## Description
The user registration form successfully accepts passwords that are only 4 characters long, bypassing the security requirement that passwords must contain a minimum of 8 characters.

## Steps to Reproduce
1. Navigate to `https://staging.example.com/signup`.
2. Enter a valid email and name.
3. Enter a 4-character password (e.g., `1234`) into the Password field.
4. Click the "Register" button.

## Expected Result
The system should display an inline validation error stating *"Password must be at least 8 characters long"* and prevent account creation.

## Actual Result
The account is created successfully, and the user is redirected to the welcome dashboard with an insecure 4-character password.

## Evidence / Attachments
- `short_password_accepted.png`
