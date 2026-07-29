# Privacy Policy for APS SCANNER

**Effective Date:** July 29, 2026
**Last Updated:** July 29, 2026
**App Version:** 1.0.3

---

## 1. Introduction

Welcome to **APS SCANNER** ("the App", "we", "us", "our").

This Privacy Policy describes how APS SCANNER handles your data. We built this app with a privacy-first philosophy: your scanned content, generated QR codes, and scan history stay on your device and are never uploaded to our servers — **because we have no servers**.

However, the App does use third-party libraries that may communicate with external services. This policy is fully transparent about what happens on your device and what goes over the network.

---

## 2. What Data We Collect

### Data We Collect Directly: **None**

APS SCANNER does **not** collect, transmit, or store on any external server:

- Your name, email, phone number, or any personal identifiers
- Device identifiers (Android ID, IMEI, Advertising ID)
- Location data
- Camera images or video recordings
- Contents of scanned QR codes or barcodes
- OCR-recognized text
- Generated QR code designs
- Scan history records
- Usage analytics or behavioral data

### Data Stored Locally on Your Device

The App stores the following data **exclusively on your device** within Android's private application sandbox:

| Local Data | Storage Method | Purpose |
|---|---|---|
| Scan history (content, type, timestamp) | Room SQLite Database | Lets you review previously scanned codes |
| App preferences (theme, sound, vibration) | Jetpack DataStore | Remembers your settings |
| Exported files (PNG, PDF, SVG, CSV) | Device Pictures/Downloads folder | Only created when you explicitly tap "Export" |

You can permanently delete all scan history at any time using **Settings → Clear All History**. Uninstalling the app removes all locally stored data.

---

## 3. Third-Party Libraries and Network Activity

APS SCANNER does **not** include advertising SDKs, analytics SDKs, or user-tracking frameworks. However, the following third-party components are used:

### 3.1 Google ML Kit (Barcode Scanning & Text Recognition)

- **What it does:** Provides on-device barcode scanning and OCR text recognition.
- **How it works:** ML Kit processes camera frames **entirely on your device** using machine learning models. Scanned content is never sent to Google.
- **Network activity:** ML Kit is delivered through **Google Play Services**, which may automatically download or update ML models in the background. This download is handled by Google Play Services, not by our App. We have disabled ML Kit's optional diagnostic telemetry (`mlkit.telemetry.disable = true`).
- **Google's policy:** Google Play Services is governed by [Google's Privacy Policy](https://policies.google.com/privacy). We do not control Google Play Services' own data practices.

### 3.2 ZXing Core

- **What it does:** Generates QR code bitmaps and SVG images.
- **Network activity:** **None.** ZXing operates entirely offline with zero network calls.

### 3.3 Coil (Image Loading)

- **What it does:** Efficiently loads and displays images within the app UI.
- **Network activity:** In our app, Coil is used **only for local images** (device gallery photos for logo import). It does not load images from the internet.

### 3.4 AndroidX Libraries (Jetpack)

- Room, DataStore, CameraX, Compose, Lifecycle, Navigation — all operate locally on-device with no network activity.

---

## 4. Android Permissions

| Permission | Why It's Needed | Data Sent Over Network? |
|---|---|---|
| `CAMERA` | Real-time QR/barcode scanning via CameraX + ML Kit | **No** — frames processed on-device only |
| `INTERNET` | Opening scanned web links in your browser; opening the Privacy Policy page | **No user data sent** — only used to launch external browser with a URL you chose to open |
| `VIBRATE` | Optional haptic feedback when a code is detected | **No** |
| `WRITE_EXTERNAL_STORAGE` (Android 9 and below only) | Saving exported QR images and CSV files to device storage | **No** |

### Important Notes on Permissions

- **Camera:** Frames are held in temporary memory during scanning and immediately discarded. No images or video are saved unless you explicitly export a generated QR code.
- **Internet:** The App itself makes **zero outgoing HTTP requests**. The INTERNET permission exists solely so Android can launch your default browser when you tap "Open" on a scanned URL or "Privacy Policy" in Settings. The App does not fetch, download, or upload any data.
- **Camera is optional:** The `android.hardware.camera` feature is declared as `required="false"`. The App can function (QR generation, history viewing) without a camera.

---

## 5. Data Sharing

We do **not** share your data with any third parties because we do not have access to your data. All processing happens on your device.

The only scenario where data leaves your device is when **you explicitly choose** to:

- **Open a scanned URL** → Your device's browser opens the link
- **Share scan results** → Android's share sheet sends the text to an app you select
- **Export files** → Files are saved to your device's local storage

In each case, you initiate the action and control where the data goes.

---

## 6. Data Safety Declaration (Google Play)

| Category | Declaration |
|---|---|
| **Data collected** | No user data collected |
| **Data shared with third parties** | No data shared |
| **Data encrypted in transit** | Not applicable (no data transmitted by the App) |
| **Data deletion** | Users can delete all local data via Settings → Clear All History |
| **Advertising or marketing** | No ads, no ad SDKs |
| **Analytics or tracking** | No analytics SDKs; ML Kit telemetry disabled |

> **Disclosure:** Google Play Services (required for ML Kit) operates independently and is governed by Google's own privacy policy. Google Play Services may collect device diagnostics, crash reports, or performance data as part of its normal operation. This is outside the App's control. For details, see [Google's Privacy Policy](https://policies.google.com/privacy).

---

## 7. Cloud Backup

APS SCANNER has **disabled Android Auto Backup** (`android:allowBackup="false"`). Your scan history and app preferences are **not** backed up to Google Drive or any cloud service. The Room database and DataStore files are explicitly excluded from both cloud backup and device-to-device transfer backup rules.

---

## 8. Security Measures

- **Application Sandbox:** All local data is isolated within Android's per-app security sandbox.
- **Device Encryption:** Data at rest is protected by your device's built-in encryption (if enabled).
- **URL Safety Checks:** The App includes a built-in URL security scanner that warns you about suspicious, phishing, or potentially dangerous links before you open them.
- **Dangerous URI Blocking:** Schemes like `intent://`, `javascript:`, `file://`, and `content://` are automatically blocked when detected in scanned codes.
- **Release Build Protection:** Sensitive debug logging is disabled in production builds.
- **No Cloud Backup:** Prevents unintended data leakage through backup services.

---

## 9. Children's Privacy (COPPA Compliance)

APS SCANNER does not collect personal information from any user, including children under 13. Because no personal data is collected, stored, or transmitted, the App is safe for users of all ages.

---

## 10. Changes to This Privacy Policy

We may update this Privacy Policy when we release new app versions or to reflect changes in Google Play policies. The updated policy will be published at the URL below with a revised "Last Updated" date. Continued use of the App after changes constitutes acceptance of the updated policy.

---

## 11. Contact

If you have questions or concerns about this Privacy Policy:

- **Developer Email:** alibekplus@gmail.com
- **GitHub:** [https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy](https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy)

---

*By installing and using APS SCANNER, you acknowledge that you have read and understood this Privacy Policy.*
