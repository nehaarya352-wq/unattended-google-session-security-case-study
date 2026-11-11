# Unattended Google Account Session Security Case Study

## Overview

This project presents a cybersecurity case study based on an observed incident involving an unattended Google account session on a shared university workstation.

The incident demonstrated how an active authenticated browser session can expose personal information when a user forgets to sign out from a shared computer.

## Objectives

- Understand the security risks of unattended authenticated sessions.
- Study session management and authentication concepts.
- Identify potential information disclosure risks.
- Evaluate the security implications of shared workstations.
- Recommend preventive security controls.

## Incident Summary

During a university computer laboratory session, an existing Google account session was found active on a shared workstation.

The browser allowed access to multiple Google services and account-management information without requiring a fresh login.

The situation demonstrated the potential consequences of leaving an authenticated account unattended.

**Note:** This case study anonymizes the incident. No personal information, account credentials, photographs, contact details, or identifiable device information are included.

## Key Security Observations

1. An authenticated Google session remained active.
2. Multiple Google services were accessible.
3. Account-associated device information was visible.
4. Personal information could potentially be exposed.
5. Two-Step Verification was not enabled on the observed account.

## Security Concepts

- Session Management
- Authentication and Authorization
- Information Disclosure
- Physical Security
- Shared Workstation Security
- Multi-Factor Authentication

## Potential Risks

- Unauthorized access to personal information.
- Exposure of private documents and photographs.
- Contact information disclosure.
- Social engineering opportunities.
- Privacy and confidentiality violations.

## Recommended Security Controls

- Always sign out after using shared computers.
- Use guest browser profiles or isolated sessions.
- Implement automatic session cleanup.
- Enable Two-Step Verification.
- Avoid saving credentials on public workstations.
- Apply institutional endpoint security policies.

## Conclusion

This case study highlights the importance of secure session management and user awareness.

An authenticated session left unattended on a shared computer can create privacy and information security risks, even without password theft or sophisticated exploitation.

## Disclaimer

This project is intended strictly for educational and cybersecurity awareness purposes. The observations are anonymized. No unauthorized testing, data collection, account modification, or exploitation is presented as part of this project.

The incident does not establish a vulnerability in Google's infrastructure.
