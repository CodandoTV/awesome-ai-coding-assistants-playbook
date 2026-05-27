# OWASP MASTG (Mobile Application Security Testing Guide) - iOS

Specific testing techniques for iOS security assessment.

## Static Analysis (SAST)

### 1. Info.plist
Audit app permissions, background modes, and URL schemes.
- **Check:** `NSAppTransportSecurity`, `NSCameraUsageDescription`, etc.

### 2. Disassembly
Analyze Mach-O binary using `Ghidra`, `Hopper`, or `objdump`.
- **Check:** Identify symbols, hardcoded secrets, weak crypto.

### 3. Entitlements
Review `.entitlements` file for sensitive capabilities.
- **Check:** `com.apple.developer.aps-environment`, `keychain-access-groups`.

## Dynamic Analysis (DAST)

### 1. Frida / Objection
Intercept methods and bypass local security controls (Jailbreak Detection, SSL Pinning).
- **Check:** `ios jailbreak disable`, `ios sslpinning disable`.

### 2. Network Interception
Intercept traffic using Burp Suite or OWASP ZAP.
- **Check:** Install Burp CA profiles, configure proxy.

### 3. Keychain Inspection
Dump keychain items using `keychain-dumper` or `objection`.
- **Check:** Access groups, accessibility flags.

## Platform Specifics

### 1. App Sandbox
Verify files are stored within the sandbox and use appropriate protection.
- **Check:** `NSFileProtectionComplete`, `NSFileProtectionCompleteUntilFirstUserAuthentication`.

### 2. Biometric Auth
Test LocalAuthentication implementation.
- **Check:** `LAContext` usage, fallback mechanisms.
