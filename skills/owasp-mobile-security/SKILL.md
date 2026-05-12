---
name: owasp-mobile-security
description: Security analysis and testing for Android and iOS apps based on OWASP Mobile Application Security (MAS). Use when verifying security requirements (MASVS), performing security tests (MASTG), or understanding mobile vulnerabilities (MASWE).
---

# OWASP Mobile Security Skill

This skill provides specialized guidance for Android and iOS mobile app security, based on the OWASP MAS project.

## Workflow: Security Review

Follow these steps when performing a mobile security audit or verifying a feature's security.

1.  **Define Requirements (MASVS):**
    - Use [references/masvs.md](references/masvs.md) to identify the relevant security controls for your feature or app.
    - Determine the MASVS level (L1 Standard, L2 High Security, or Resilience).

2.  **Audit Source Code / Configuration (SAST):**
    - For Android, use [references/mastg-android.md](references/mastg-android.md) (Static Analysis section).
    - For iOS, use [references/mastg-ios.md](references/mastg-ios.md) (Static Analysis section).

3.  **Perform Runtime Testing (DAST):**
    - Follow the Dynamic Analysis procedures in the platform-specific guides to bypass local controls or intercept traffic.

4.  **Finalize & Report:**
    - Use [references/checklist.md](references/checklist.md) to track progress and ensure all categories are covered.

## Quick References

- **MASVS Categories:** [references/masvs.md](references/masvs.md)
- **Android Testing Guide:** [references/mastg-android.md](references/mastg-android.md)
- **iOS Testing Guide:** [references/mastg-ios.md](references/mastg-ios.md)
- **Security Checklist:** [references/checklist.md](references/checklist.md)

## Example Tasks

- "Audit this AndroidManifest.xml for insecure exported components."
- "Show me how to bypass SSL pinning on iOS using Frida."
- "What are the MASVS requirements for secure biometric authentication?"
- "Check this code for PII data leakage in system logs."
