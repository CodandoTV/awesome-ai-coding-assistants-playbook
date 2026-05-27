# OWASP MASVS (Mobile Application Security Verification Standard)

The MASVS defines 8 security verification categories for mobile apps.

## Categories

### 1. MASVS-STORAGE (Storage)
Secure storage of sensitive data (PII, credentials).
- **Requirement:** Minimize data footprint; use platform secure storage (KeyStore/Keychain).
- **Verification:** Check for data in logs, shared prefs, databases, and temporary files.

### 2. MASVS-CRYPTO (Cryptography)
Proper use of cryptographic primitives.
- **Requirement:** Use strong, modern algorithms (AES-GCM, RSA-2048+); avoid custom crypto.
- **Verification:** Identify hardcoded keys, weak IVs, and insecure random number generation.

### 3. MASVS-AUTH (Authentication/Authorization)
Secure user identity and session management.
- **Requirement:** Enforce server-side validation; implement biometric/MFA best practices.
- **Verification:** Check session timeout, secure token handling, and MFA enforcement.

### 4. MASVS-NETWORK (Network)
Secure data transit between app and server.
- **Requirement:** Use TLS for all communication; implement certificate pinning for high-security.
- **Verification:** Check for cleartext traffic (HTTP), weak TLS versions, and pinning bypass.

### 5. MASVS-PLATFORM (Platform Interaction)
Secure use of OS APIs and Inter-Process Communication (IPC).
- **Requirement:** Secure Intents, WebViews, and permissions; prevent UI data leakage.
- **Verification:** Audit exported components, JavaScript bridges, and notification content.

### 6. MASVS-CODE (Code Quality)
Secure coding practices and dependency management.
- **Requirement:** Validate all inputs; keep dependencies updated; use compiler security features.
- **Verification:** Check for outdated libraries, debug symbols, and insecure logic.

### 7. MASVS-RESILIENCE (Resilience)
Protection against reverse engineering and tampering.
- **Requirement:** Implement root/jailbreak detection, obfuscation, and anti-debugging.
- **Verification:** Verify if the app runs on rooted/jailbroken devices and if code is obfuscated.

### 8. MASVS-PRIVACY (Privacy)
User data protection and transparency.
- **Requirement:** Minimize collection; provide clear policies and consent mechanisms.
- **Verification:** Audit data sent to 3rd party SDKs and analytics.
