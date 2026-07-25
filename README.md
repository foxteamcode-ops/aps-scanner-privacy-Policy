# Privacy Policy for APS SCANNER (QR Studio)

**Effective Date:** July 25, 2026  
**Last Updated:** July 25, 2026  
**Version:** 1.2

Welcome to **APS SCANNER** (also referred to as **QR Studio**, **the Application**, **we**, **us**, or **our**).

Your privacy is important to us. This Privacy Policy explains how APS SCANNER handles user data, permissions, and security.

---

# 1. Data Collection

APS SCANNER does **not collect, store, transmit, sell, or share** your personal information.

The application performs its core functionality locally on your Android device.

We do **not** collect:

- Name
- Email address
- Phone number
- Device identifiers (Android ID, IMEI, Advertising ID)
- Location data
- Contacts
- Camera images or videos
- QR code or barcode contents
- OCR-recognized text
- Generated QR codes
- Scan history

Barcode scanning, QR generation, text recognition, and image processing are performed locally on the device.

---

# 2. Permissions

APS SCANNER requests only the permissions required for its core functionality.

| Permission | Purpose |
|------------|---------|
| **Camera** (`android.permission.CAMERA`) | Used to scan QR codes and barcodes in real time. Camera frames are processed locally and are never recorded or uploaded. |
| **Vibrate** (`android.permission.VIBRATE`) | Provides optional haptic feedback after a successful scan or QR code generation. |
| **MediaStore Storage Access** | Used only when you choose to save or export QR codes or scan history. Files are created only after your explicit action and are stored on your device. |

APS SCANNER does not access your personal files without your action.

The application uses Android's modern **Scoped Storage** system and does not request the legacy `WRITE_EXTERNAL_STORAGE` permission on supported Android versions.

---

# 3. Third-Party Services

APS SCANNER does not include:

- Advertising SDKs
- Analytics SDKs
- Tracking SDKs
- Telemetry services

The application does not send usage data or personal information to external servers.

APS SCANNER uses Google's on-device ML Kit APIs for barcode recognition. Barcode processing is performed locally on the device.

---

# 4. Children's Privacy

APS SCANNER does not knowingly collect personal information from children or users of any age.

Because the application does not collect personal data, no personal information is transmitted or stored.

---

# 5. Data Storage and Security

Application data is stored locally on your device.

This may include:

- Scan history (Room Database)
- Application settings (DataStore)
- QR codes or exported files that you choose to save

Data is protected by Android's application sandbox.

If device encryption is enabled, locally stored data also benefits from Android's storage encryption.

APS SCANNER does not upload any of this information to external servers.

---

# 6. Changes to This Privacy Policy

This Privacy Policy may be updated to reflect changes in application functionality, Android platform requirements, or Google Play policies.

The latest version will always be available in the project's GitHub repository.

---

# 7. Contact

If you have any questions regarding this Privacy Policy, you can contact us:

**Developer Email**

alibekplus@gmail.com

**GitHub Repository**

https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy

---

# Google Play Privacy Summary

- No personal data is collected.
- No personal data is transmitted.
- No advertising.
- No analytics.
- No tracking.
- No telemetry.
- Camera permission is used only for QR and barcode scanning.
- Exported files are created only after explicit user action.
- All core functionality operates locally on the device.
- User data remains on the device.

By using APS SCANNER, you acknowledge this Privacy Policy.
