# Privacy Policy for APS SCANNER (QR Studio)

**Effective Date:** July 25, 2026  
**Last Updated:** July 25, 2026  
**App Version:** 1.0.0  

Welcome to **APS SCANNER** (also referred to as **QR Studio**, **the Application**, **we**, **us**, or **our**).

Your privacy is our top priority. This Privacy Policy explains how APS SCANNER handles user data, permissions, and security in strict compliance with Google Play Developer Policies and Data Safety requirements.

---

## 1. Zero Data Collection & Local Processing

APS SCANNER does **not collect, store, transmit, sell, or share** any of your personal information.

The application performs 100% of its core functionality **locally on your Android device** without relying on external servers or cloud services.

We do **not** collect or transmit:

- Personal Identifiable Information (Name, Email address, Phone number)
- Device identifiers (Android ID, IMEI, MAC Address, Advertising ID)
- Location data (GPS or IP-based location)
- Contact books or personal media
- Camera frames, images, or recorded video
- QR code or barcode contents
- OCR-recognized text
- Custom-generated QR codes and design assets
- Scan history records

All barcode scanning, QR generation, text recognition (OCR), and image rendering operate entirely offline on your device.

---

## 2. Android Permissions

APS SCANNER requests only the minimal Android permissions necessary to deliver its core functionality:

| Permission | Purpose |
|------------|---------|
| **Camera** (`android.permission.CAMERA`) | Used exclusively to scan QR codes and barcodes in real time using on-device ML Kit APIs. Camera frames are processed in temporary memory and are **never recorded, stored, or uploaded**. |
| **Vibrate** (`android.permission.VIBRATE`) | Provides optional haptic tactile feedback when a QR code or barcode is detected. |
| **Internet** (`android.permission.INTERNET`) | Used solely to allow you to launch scanned web links (`http://` or `https://`) or open the Privacy Policy in your external default web browser upon your explicit action. **No personal data is collected or sent over the internet by the app.** |
| **MediaStore Access** | Used only when you explicitly choose to export or save generated QR code images (PNG, PDF, SVG) or CSV scan history to your device's storage. |

The application utilizes Android's modern **Scoped Storage** framework and does not request legacy `WRITE_EXTERNAL_STORAGE` permissions on supported Android versions.

---

## 3. Third-Party Services & Libraries

APS SCANNER is designed to be privacy-first. The application does **not** integrate:

- Advertising SDKs or Ad Networks
- User Analytics SDKs (e.g., Firebase Analytics, Google Analytics)
- Behavior Tracking or Telemetry SDKs
- Social media tracking plugins

APS SCANNER uses Google's on-device **ML Kit Barcode Scanning** and **Text Recognition** APIs. All machine learning inference is performed locally on the device hardware without sending data to Google or any third party.

---

## 4. Children's Privacy

APS SCANNER is safe for users of all ages, including children. Because the application does **not collect or request any personal information**, no data from children is ever gathered, processed, or shared.

---

## 5. Local Data Storage & Security

Any data created while using the application remains strictly on your device:

- **Scan History**: Saved locally in a private Room SQLite Database.
- **App Preferences**: Stored locally in Android Jetpack DataStore.
- **Exported Files**: Saved to your public Pictures/Downloads directory only when you tap export.

All local data is isolated within Android's application sandbox and protected by standard device-level encryption. You can permanently delete your entire scan history at any time using the "Clear All History" feature in the app.

---

## 6. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect platform changes, new features, or updated Google Play policies. The most current version will always be published in the project's official GitHub repository.

---

## 7. Contact Information

If you have any questions, feedback, or concerns regarding this Privacy Policy, please contact:

- **Developer Email:** alibekplus@gmail.com  
- **GitHub Repository:** [https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy](https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy)

---

## Google Play Data Safety Summary

- **Data Collected:** None (0%)
- **Data Shared:** None (0%)
- **Advertising:** No Ads
- **Analytics / Tracking:** None
- **Encryption in Transit:** N/A (No network transmission of user data)
- **Data Deletion:** User can clear all local history directly inside the app

*By using APS SCANNER, you acknowledge and agree to this Privacy Policy.*
