# Privacy Policy for APS SCANNER (QR Studio)

**Effective Date:** July 25, 2026  
**Last Updated:** July 25, 2026  
**Version:** 1.1

Welcome to **APS SCANNER** (also referred to as “QR Studio”, “the Application”, “we”, “us”, or “our”). We are committed to protecting your privacy and securing your data. This Privacy Policy explains how the Android application handles user data, permissions, and security.

---

## 1. Zero Personal Data Collection (100 % On‑Device Processing)

APS SCANNER operates entirely **on‑device**. We **do not collect, store, transmit, sell, or share** any of the following:

- Personal information (name, email, phone, etc.)
- Scanned barcode or QR‑code contents
- Generated QR graphics (PNG, SVG, PDF)
- OCR‑extracted text
- Device identifiers (IMEI, Android ID, Advertising ID)

All barcode analysis, computer‑vision calculations (Google ML Kit), text recognition, and vector QR rendering occur locally on your Android device.

---

## 2. Device Permissions Usage

The Application requests only the permissions required to provide its core functionality. Each permission is used **exclusively** for the purpose described below and never for data collection or tracking.

| Permission | Why it is needed | Privacy Assurance |
|------------|------------------|-------------------|
| **Camera** (`android.permission.CAMERA`) | Captures real‑time camera frames for QR‑code and barcode recognition. | Video frames are processed in volatile memory only; they are **never recorded, saved, or uploaded**. |
| **Vibrate** (`android.permission.VIBRATE`) | Provides a short haptic feedback when a scan succeeds or a QR code is generated. | Vibration is triggered locally; no data is transmitted. |
| **Storage Access** (via **MediaStore** API) | Exports generated QR codes (PNG, SVG, PDF) and scan‑history files (CSV) to the device’s public `Pictures/QRStudio` and `Downloads/QRStudio` folders **after explicit user action** (e.g., tapping “Export”). | The app only writes files that you have created. It does **not read** other media files, nor does it upload any exported files. |
| *(No `WRITE_EXTERNAL_STORAGE` request on Android 10+; Scoped Storage is used.)* |  | |

---

## 3. Third‑Party Services & Tracking SDKs

APS SCANNER **contains no third‑party advertising, analytics, or telemetry SDKs**. There are no libraries that collect usage statistics or send data to external servers.

*If any optional debugging or crash‑reporting library (e.g., Firebase Crashlytics) is added in the future, it will be disclosed in this section along with the exact data it collects.*

---

## 4. Children’s Privacy

We comply with the **Children’s Online Privacy Protection Act (COPPA)** and Google Play **Families Policy**. Because the Application does **not collect any personal data** from anyone, it is safe for users of all ages, including children under 13.

---

## 5. Security

All scan history, generated QR graphics, and user preferences are stored locally:

- **Room Database** – stores scan records in an isolated SQLite database.
- **DataStore (Proto)** – stores user settings (e.g., theme choice).

The data remains on the device and is protected by the Android operating system. If you enable device‑level encryption (e.g., full‑disk encryption or encrypted Room), the stored data is additionally encrypted. No data is transmitted off‑device.

---

## 6. Updates to This Privacy Policy

We may update this Privacy Policy to reflect changes in Android OS guidelines, Google Play policies, or app functionality. Any updates will be posted on the **GitHub repository** linked below, and the “Effective Date” will be revised accordingly.

---

## 7. Contact Us

If you have any questions, concerns, or suggestions regarding this Privacy Policy or the Application, please contact us at:

- **Developer / Support Email:** alibekplus@gmail.com
- **GitHub Repository:** [aps‑scanner‑privacy‑Policy](https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy)

---

### Summary for Google Play Review

- No personal data is collected, stored, or transmitted.
- Permissions are limited to **Camera**, **Vibrate**, and **MediaStore‑based storage access** (triggered only after explicit user action).
- No third‑party analytics or advertising SDKs are present.
- The app complies with COPPA and Families Policy.
- All data stays on‑device; optional encryption is used where available.

By adhering to the above, APS SCANNER meets Google Play’s privacy‑policy requirements.
