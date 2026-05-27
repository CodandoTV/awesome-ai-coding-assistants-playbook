# OWASP MASTG (Mobile Application Security Testing Guide) - Android

Specific testing techniques for Android security assessment.

## Static Analysis (SAST)

### 1. AndroidManifest.xml
Audit permissions, exported components (Activities, Services, Receivers), and debuggable flag.
- **Check:** `android:exported="true"`, `android:debuggable="true"`, excessive permissions.

### 2. Decompilation
Use `JADX` or `Apktool` to analyze Smali/Java code.
- **Check:** Hardcoded secrets, weak crypto, insecure IPC.

### 3. Native Libraries
Inspect `.so` files using `Ghidra` or `strings`.
- **Check:** Hardcoded keys, insecure logic in native code.

## Dynamic Analysis (DAST)

### 1. Frida Hooking
Intercept methods and bypass local security controls (Root Detection, SSL Pinning).
- **Check:** Bypass `isRooted()` checks, intercept `java.net.URL.openConnection`.

### 2. Network Interception
Intercept traffic using Burp Suite or OWASP ZAP.
- **Check:** Configure proxy on device/emulator, install Burp CA.

### 3. IPC Testing
Use `adb shell am` or `drozer` to interact with exported components.
- **Check:** Trigger unauthenticated Intents, SQL injection in Content Providers.

## Platform Specifics

### 1. Android KeyStore
Ensure sensitive data is stored in the hardware-backed KeyStore.
- **Check:** Use of `KeyGenParameterSpec`, hardware backing verification.

### 2. Scoped Storage
Verify app respects scoped storage and doesn't leak data.
- **Check:** `getExternalFilesDir()` vs. `getExternalStorageDirectory()`.
