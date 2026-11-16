# QA Proof of Work — iHealth Wellness Foundation

Project: User Registration and Authentication
Prepared by: Muhammad Mehboob, PM — MATIG Technologix
Date: November 2026

## Test Summary

| Module | Total | Pass | Pending |
|---|---|---|---|
| User Registration and Sign In | 183 | 115 | 68 |
| Edit Profile | 17 | 9 | 8 |
| Forgot Password | 20 | 12 | 8 |
| Grand Total | 220 | 136 | 84 |

Pass Rate: 62%

## Modules Covered

- Homepage navigation and branding
- Sign In page — validation, security, error handling
- Sign Out — session management
- Create Account — email validation, password strength
- Patient Registration — form validation, country, state, city
- Provider Registration — specialty, role, confirmation
- Internal User Registration — company email enforcement
- Recovery Question setup
- Email Verification — link expiry, resend, tamper detection
- Forgot Password — reset flow, link expiry
- Edit Profile — field updates, validation

## Test Types Applied

- Functional testing
- UI and design validation against Figma specs
- Negative testing — invalid inputs, empty fields
- Security testing — SQL injection, XSS, account lockout
- Responsive testing — 375px mobile viewport
- Session management testing
- Email flow testing

## Sample Test Cases

| ID | Module | Description | Status |
|---|---|---|---|
| TC_SI_032 | Sign In | SQL injection in email field does not break app | Pending |
| TC_SI_033 | Sign In | XSS script in email field is sanitized | Pending |
| TC_SI_034 | Sign In | Account lockout after 5 failed login attempts | Pending |
| TC_CA_049 | Create Account | Already registered email is rejected | Pass |
| TC_EV_109 | Email Verification | Tampered verification link is rejected | Pending |
| TC_IU_088 | Internal User | Non-company email rejected for internal registration | Pass |
