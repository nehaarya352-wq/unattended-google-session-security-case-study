# Detailed Security Case Study

## 1. Introduction

Authentication allows users to access digital services after their identity has been verified. However, security risks can arise when an authenticated session remains active on a shared workstation.

This case study examines an observed situation in which a Google account was left signed in on a university computer, making account-associated services accessible to another person using the same workstation.

## 2. Problem Statement

A student left a shared university workstation without signing out of their Google account.

The browser retained the authenticated session, allowing access to multiple Google services without requiring fresh authentication.

This created a potential risk of unauthorized access to personal information.

## 3. Technical Observations

The following security conditions were observed:

- An existing Google session was active.
- Gmail, Google Photos and Google Contacts were accessible.
- Google Account security settings were accessible.
- Account-associated device information was visible.
- Two-Step Verification was not enabled.

No personal information or identifying details are reproduced in this report.

## 4. Technical Explanation

### 4.1 Authenticated Session

After successful authentication, a browser can maintain a session using session-related credentials, such as cookies.

These allow a user to continue accessing supported services without repeatedly entering their password.

If the user leaves the workstation without signing out, another person with access to that browser may be able to use the existing session.

### 4.2 Authentication

Authentication verifies the identity of a user.

Examples include passwords, passkeys, fingerprints and verification codes.

### 4.3 Authorization

Authorization determines which resources and actions an authenticated user is permitted to access.

### 4.4 Multi-Factor Authentication

Multi-Factor Authentication adds another verification factor during supported authentication processes.

However, MFA does not automatically prevent misuse of an already-authenticated and accessible session.

## 5. Potential Security Impact

### Confidentiality

Private information, documents, photographs and contact details may become accessible.

### Integrity

If an exposed session permits account modifications, an unauthorized person could potentially alter account information.

### Availability

If an exposed session permits certain account-management actions, unauthorized changes could interfere with account access.

These are potential consequences, not actions demonstrated during the observation.

## 6. Root Cause Analysis

The primary contributing condition was an authenticated account session remaining active on a shared workstation.

Additional contributing factors may include:

- Failure to sign out.
- Insufficient workstation session isolation.
- Lack of automatic browser session cleanup.
- Limited awareness of shared-computer security risks.

The absence of Two-Step Verification was an additional security concern, but it was not the direct cause of the existing session remaining active.

## 7. Mitigation Strategies

1. Sign out of all personal accounts after using shared computers.
2. Use guest browser sessions.
3. Clear browser data between users.
4. Implement automatic workstation session timeouts.
5. Enable Two-Step Verification or passkeys.
6. Avoid saving passwords on shared devices.
7. Educate students about account security.

## 8. Ethical Considerations

This case study is based on a real-world security observation.

The account owner's personal information was not intentionally collected, retained, or published.

No credentials, contact information, photographs, account identifiers or screenshots of private information are included.

The purpose is to understand the security implications of unattended sessions and recommend preventive controls.

## 9. Conclusion

The incident demonstrates that account security involves more than strong passwords.

Session management, physical workstation security and user awareness are equally important.

Educational institutions should implement suitable security policies to reduce the risks associated with shared computer environments.

## 10. References

- Google Account Help: https://support.google.com/accounts/
- OWASP Session Management Cheat Sheet: https://cheatsheetseries.owasp.org/cheatsheets/Session_Management_Cheat_Sheet.html
- OWASP Authentication Cheat Sheet: https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html
