# App Risk Auditor (PS-01)
Kotlin, zero dependencies, fully on-device and offline.
Build: push to GitHub -> Actions -> artifact `AppRiskAuditor-apk` (app-debug.apk). Or Android Studio: open folder, Run. Or `gradle assembleDebug`.
Install, open, allow notifications. Special access detection uses Settings.Secure, DevicePolicyManager and AppOps (no root/ADB).
Not implemented (stretch): hash lookup, manifest checks, ML model, PDF export.
