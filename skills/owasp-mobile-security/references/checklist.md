# Mobile Security Assessment Checklist

A combined checklist based on MASVS and MASTG.

## 1. Storage (MASVS-STORAGE)
- [ ] No sensitive data in logs (adb logcat / Console.app).
- [ ] No PII/credentials in SharedPrefs/UserDefaults/DBs.
- [ ] No data leaked via UI (Keyboard cache, snapshots).
- [ ] Secure use of KeyStore (Android) or Keychain (iOS).

## 2. Cryptography (MASVS-CRYPTO)
- [ ] No hardcoded keys/secrets in binary.
- [ ] Strong algorithms only (AES-GCM, RSA-2048+, SHA-256+).
- [ ] Proper initialization vectors (non-predictable).
- [ ] Key management follows platform best practices.

## 3. Auth & Session (MASVS-AUTH)
- [ ] Session tokens handled securely (HTTPOnly, Secure flags for cookies).
- [ ] MFA/Biometrics used correctly.
- [ ] Account lockout / rate limiting on server-side.
- [ ] No sensitive data in URL/GET params.

## 4. Network (MASVS-NETWORK)
- [ ] All traffic via TLS (HTTPS).
- [ ] No weak TLS versions or cipher suites.
- [ ] SSL Pinning implemented for high-security.
- [ ] Proper handling of certificate errors.

## 5. Platform (MASVS-PLATFORM)
- [ ] No exported components without permissions.
- [ ] WebViews use secure configuration (JavaScript disabled if not needed).
- [ ] Intents/URL Schemes validated on receipt.
- [ ] No sensitive info in push notifications.

## 6. Code & Resilience (MASVS-CODE/RESILIENCE)
- [ ] Binary obfuscated (ProGuard/R8 or Swift/LLVM).
- [ ] Root/Jailbreak detection implemented.
- [ ] Anti-debugging / Anti-tamper mechanisms active.
- [ ] Third-party libraries are up-to-date.

## 7. Privacy (MASVS-PRIVACY)
- [ ] Clear privacy policy provided.
- [ ] User consent for sensitive data collection.
- [ ] Minimal data sent to analytics/3rd parties.
- [ ] Proper handling of data deletion requests.
