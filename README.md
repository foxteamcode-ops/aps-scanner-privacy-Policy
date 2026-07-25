# Privacy Policy for APS SCANNER (QR Studio)

**Effective Date:** July 25, 2026  
**Last Updated:** July 25, 2026  

Welcome to **APS SCANNER** (also referred to as "QR Studio", "the Application", "we", "us", or "our"). We are committed to maintaining 100% user privacy and data security. 

This Privacy Policy explains how our Android application handles user data, permissions, and security.

---

## 1. Zero Personal Data Collection (100% On-Device Processing)

APS SCANNER operates entirely **on-device**. We do **NOT** collect, store, transmit, sell, or share any personal information, scanned barcode contents, generated QR graphics, OCR extracted text, or device identifiers to external servers or third parties.

All barcode analysis, computer vision calculations (using Google ML Kit), text recognition, and vector QR rendering occur locally on your Android device.

---

## 2. Device Permissions Usage

To provide core barcode scanning and export functionalities, the Application requests the following Android permissions:

### A. Camera Permission (`android.permission.CAMERA`)
- **Purpose:** Used strictly to capture real-time camera frames for QR code and barcode recognition.
- **Privacy Assurance:** Camera video streams are analyzed in volatile memory on your device and are never recorded, saved, or uploaded to any remote server.

### B. Storage Access (`MediaStore` API)
- **Purpose:** Used solely to export generated QR codes (PNG, SVG, PDF) and scan history exports (CSV) into your device’s public `Pictures/QRStudio` and `Downloads/QRStudio` folders upon your explicit action.
- **Privacy Assurance:** The Application only writes exported graphics created by you and does not scan or upload your private photos.

---

## 3. Third-Party Services & Tracking SDKs

APS SCANNER contains **NO third-party advertising SDKs**, **NO analytics trackers**, and **NO telemetry frameworks**. We do not track your activity across other apps or websites.

---

## 4. Children’s Privacy Policy

Our Application complies with the Children’s Online Privacy Protection Act (COPPA) and Google Play Families Policy. Because APS SCANNER does not collect any personal data from anyone, it is 100% safe for users of all ages, including children under 13.

---

## 5. Security

Because all scanned history and studio designs remain stored within your device's local Android isolated storage (SQLite Room Database and DataStore), your data security depends on protecting access to your physical Android device.

---

## 6. Changes to This Privacy Policy

We may update our Privacy Policy from time to time to maintain compliance with updated Android OS guidelines and Google Play policies. Any updates will be posted on this GitHub repository page.

---

## 7. Contact Us

If you have any questions or suggestions about our Privacy Policy or APS SCANNER, please feel free to contact us at:

- **Developer / Support Email:** alibekplus@gmail.com
- **GitHub Repository:** [aps-scanner-privacy-Policy](https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy)
