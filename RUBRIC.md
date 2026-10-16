# Scoring rubric (score = sum of points, capped at 100)
Bands: Low 0-24, Medium 25-49, High 50-74, Critical 75-100. High/Critical always list >=3 reasons.

| Special access | Points |
|---|---|
| Accessibility service enabled / declared only | 30 / 6 |
| Device admin active | 25 |
| Notification listener enabled | 20 |
| Overlay allowed | 15 |
| Install-packages declared | 10 |
| Usage access allowed / declared | 6 / 3 |

Dangerous permissions (granted = full points, declared only = 30%): READ_SMS 15, RECEIVE_SMS 12, SEND_SMS 10, MANAGE_EXTERNAL_STORAGE 10, READ_CALL_LOG 8, BACKGROUND_LOCATION 8, READ_CONTACTS 7, RECORD_AUDIO 7, CAMERA 6, FINE_LOCATION 5, CALL_PHONE 4, phone state/numbers 3, media/storage read 3, battery-opt exemption 3, boot 2, INTERNET 1.

Combination rules: SMS + INTERNET + BOOT from non-store source +20; accessibility + overlay +20; device admin on non-security app +15; context mismatch (torch/calculator/wallpaper... with SMS/contacts/call log) +15; sideloaded +5.
Install monitoring + permission diff: PackageReceiver rescans on install/update and notifies on High/Critical or newly added sensitive permissions.
