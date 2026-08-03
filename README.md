# Privacy Policy for APS SCANNER

**Effective Date:** July 29, 2026  
**Last Updated:** August 03, 2026  
**App Version:** 1.0.4

---

# 1. Introduction

Welcome to **APS SCANNER** ("the App", "we", "us", or "our").

APS SCANNER is designed with a **privacy-first** approach. All scanning, QR code generation, OCR recognition, and history management are performed locally on your device.

We do **not** operate any servers, and we do **not** collect, transmit, or store your personal information.

This Privacy Policy explains what information the App stores locally, how it uses Android permissions, and how third-party libraries function.

---

# 2. Information We Collect

## Personal Data

APS SCANNER does **not** collect, store, or transmit:

- Name
- Email address
- Phone number
- Home address
- Device identifiers
- Android ID
- Advertising ID
- IMEI
- Location data
- Contacts
- Camera photos
- Videos
- Scan contents
- OCR recognized text
- Generated QR codes
- Analytics
- Crash reports
- Usage statistics

---

## Data Stored Locally

The following information is stored **only on your device**.

| Data | Storage |
|------|---------|
| Scan history | Room Database |
| User settings | Jetpack DataStore |
| Theme preferences | Jetpack DataStore |
| Automation settings | Jetpack DataStore |
| Security settings | Jetpack DataStore |
| Generated QR codes | Local storage (only if exported) |
| Exported PNG/PDF/SVG/CSV files | Device storage |

No local data is uploaded to any server.

You can delete all stored history at any time through:

**Settings → Clear All History**

Uninstalling APS SCANNER removes all application data stored inside Android's private app storage.

---

# 3. Third-Party Libraries

APS SCANNER uses several open-source and Google libraries.

## 3.1 Google ML Kit

Purpose:

- Barcode scanning
- QR code recognition
- OCR (Text Recognition)

Processing is performed **entirely on-device**.

Scanned content is **never uploaded** to Google or to our servers.

Google Play Services may download updated ML models automatically.

Google's Privacy Policy applies to Google Play Services.

---

## 3.2 ZXing

Purpose:

- QR code generation

Network activity:

**None**

ZXing works completely offline.

---

## 3.3 AndroidX Libraries

APS SCANNER uses AndroidX libraries including:

- CameraX
- Room
- DataStore
- Lifecycle
- Navigation
- Jetpack Compose

These libraries process data locally.

They do not collect or transmit user information.

---

## 3.4 Coil

APS SCANNER uses **Coil** only for displaying images selected by the user.

Network activity:

**None**

Images remain on your device and are never uploaded.

---

# 4. Automatic Features

APS SCANNER includes optional automation features.

Both are **disabled by default**.

| Feature | Default | Description |
|----------|----------|-------------|
| Auto Copy | Off | Automatically copies scan results to the clipboard after scanning |
| Auto Open Links | Off | Automatically opens scanned URLs after security validation |

These features can be enabled or disabled at any time.

---

# 5. Android Permissions

| Permission | Purpose |
|------------|---------|
| CAMERA | Scan QR codes and barcodes |
| INTERNET | Open scanned web links, display the Privacy Policy, and support required libraries |
| VIBRATE | Optional vibration feedback |
| WRITE_EXTERNAL_STORAGE (Android 9 and below only) | Export images and files |

### Camera

Camera frames are processed in memory only.

No photos or videos are saved.

---

### Internet

APS SCANNER does **not** send scan results or personal information to any server.

The INTERNET permission is used only for:

- Opening links
- Displaying the Privacy Policy
- Supporting required libraries

---

### Camera Requirement

Camera hardware is **optional**.

APS SCANNER declares:

```
android.hardware.camera
required="false"
```

The application can still generate QR codes and manage history without a camera.

---

# 6. Data Sharing

APS SCANNER does **not** share your data with any third party.

Data leaves your device only when **you choose to do so**.

Examples include:

- Opening a scanned website
- Sharing scan results through Android Share
- Copying data to the clipboard
- Exporting files

APS SCANNER never uploads your data.

---

# 7. Google Play Data Safety

| Category | Declaration |
|-----------|-------------|
| Data collected | None |
| Personal information | Not collected |
| Location | Not collected |
| Financial information | Not collected |
| Contacts | Not collected |
| Photos | Not collected |
| Files | Not collected |
| Device IDs | Not collected |
| Analytics | No |
| Crash reporting | No |
| Advertising | No |
| Third-party advertising SDKs | None |
| Data sharing | None |
| Data deletion | Available inside the app |

Google Play Services may independently collect diagnostic information according to Google's own Privacy Policy.

---

# 8. Security

APS SCANNER includes several security measures.

- Android Application Sandbox
- Local-only storage
- Device encryption (when enabled)
- URL Safety Checks (optional)
- Dangerous URI blocking
- Disabled debug logging in release builds
- No cloud synchronization

Dangerous URI schemes including:

- javascript:
- file:
- content:
- intent:

are blocked automatically.

---

# 9. Children's Privacy

APS SCANNER does not knowingly collect personal information from children.

Since the App collects no personal data, it complies with children's privacy requirements, including COPPA.

---

# 10. Changes to This Privacy Policy

This Privacy Policy may be updated when:

- new application features are added;
- Google Play requirements change;
- legal requirements change.

Updates will be published at the same URL with a revised **Last Updated** date.

---

# 11. Contact

If you have questions about this Privacy Policy, you may contact us.

**Developer Email**

alibekplus@gmail.com

**GitHub**

https://github.com/foxteamcode-ops/aps-scanner-privacy-Policy

---

By installing and using APS SCANNER, you acknowledge that you have read and understood this Privacy Policy.
