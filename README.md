# Open Store

Open Store is an Android-first Flutter app that helps you discover, download, install, update, open, and uninstall apps in one compact place.

![Open Store App Icon](assets/icons/open_store_icon.png)

## Use Case

Use Open Store when you want a simple app store experience for your curated apps, with clear app details, version visibility, and safe install checks.

## Features

- Compact app list with fast search
- App details dialog with:
  - Current installed version
  - Available version (even before download)
  - Use case, features, and permissions
- Smart actions based on app state:
  - Download
  - Pause / Resume
  - Install / Upgrade
  - Open
  - Redownload
  - Uninstall
- Download integrity verification before install
- Better retry and source handling for large APK downloads
- Smooth, lightweight transitions for a cleaner UI feel
- Open Store Admin app is hidden from normal store users
- Feedback system with status tracking
- Activity logs with copy and clear controls
- Appearance options: Light, Dark, System
- Auto refresh interval control
- Check for Open Store updates from Settings

## Permissions Required (For Users)

Open Store may require:

- `INTERNET`: To fetch app details and download APKs
- `POST_NOTIFICATIONS` (device dependent): To notify update availability
- `Install unknown apps` system setting: To install APK files

Open Store does **not** require camera, microphone, contacts, or location for normal store usage.

## How To Use

1. Open Open Store.
2. Use search or scroll to find your app.
3. Tap `Download`.
4. Tap `Install` after download completes.
5. Use `Open` for installed apps.
6. Use `Upgrade` when a newer version is available.
7. Use `Uninstall` to remove apps from device.
8. Open Feedback from any app card to report issues or suggestions.

## Feedback

Have a suggestion, bug report, or feature request?

[![Feedback Button](https://img.shields.io/badge/Feedback-Share%20Your%20Ideas-1F9BAB?style=for-the-badge)](/issues/new?labels=feedback&title=%5BFeedback%5D%20)

You can use the feedback button above to tell us what else should be added.
