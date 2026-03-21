<div align="center">
  <h1>Open Store</h1>
  <p><strong>Latest Version:</strong> 1.7.1</p>
  <p><strong>Build Date:</strong> 20-03-2026 08:20 pm</p>
  <p><strong>SHA1:</strong> 40277904e412b0d1337453ef7fb562ac6fc84be2</p>
  <p><strong>Status:</strong> Ready for Android release</p>
</div>

![Open Store App Icon](assets/icons/open_store_icon.png)

Open Store is an Android-first Flutter app that helps users discover, download, install, and update apps from one simple place.

> Checksum note: Use SHA1 only if you want to verify the downloaded APK is unchanged.

## Download URL

- Direct latest APK download: [https://github.com/paranveer/Open-Store-Apk/releases/download/open-store-admin-large-files/Open_Store_ver_1.7.1.apk](https://github.com/paranveer/Open-Store-Apk/releases/download/open-store-admin-large-files/Open_Store_ver_1.7.1.apk)
- Release page: [https://github.com/paranveer/Open-Store-Apk/releases/tag/open-store-admin-large-files](https://github.com/paranveer/Open-Store-Apk/releases/tag/open-store-admin-large-files)
- Always download the latest available Open Store version.
- If the direct file link does not work for you, open the release page and download the newest APK shown there.

## Before You Start

- If you are installing the APK manually, allow `Install unknown apps` for the browser or file manager that opens it.
- Open the app after installation and grant the required Android permissions when prompted.

## Use Case

Use Open Store when you want its main experience on Android with a simple, direct flow.

## Features

- Android release build prepared for end users
- Current app assets bundled alongside the packaged APK
- User-facing README updated for this release

## Improvements / Bug Fixes

- Auto refresh now follows the interval selected in Settings. If you choose 5 minutes, the app should no longer refresh every few seconds.
- App icons are preserved better during refreshes, so they should not keep going on and off while the catalog updates.
- Open Store update downloads now show smoother progress while downloading.
- When an update download is paused, the app now shows the downloaded amount more accurately.
- App icons now follow the same layered icon logic used in the admin app. Apps with foreground and background icon files should display more correctly.
- App names are cleaned up better, so version text and extra file-name words are less likely to appear in the store list.
- The home screen is now more compact and mobile-friendly.
- The search section was removed to reduce clutter, while the last refreshed status was kept.
- The app title and icon in the top bar were made a little larger for better visibility.
- The refresh and settings buttons now feel more responsive when tapped, with clearer press feedback and a more alive touch interaction.
- Each app section was redesigned to feel more raised and visually deeper, while staying usable on mobile screens.
- The right-side lighting effect that was covering icons on app cards was removed.
- Duplicate or unnecessary top notices were reduced so the store screen is easier to scan.
- Secondary app actions were moved into a cleaner overflow menu to keep cards shorter.
- The details view was grouped into simpler sections such as version, use case, features, permissions, and integrity.
- Feedback sharing now supports an optional gallery image attachment.
- Shared app logs are now more structured and more privacy-safe before being attached.
- Feedback images are stored separately to improve syncing reliability.
- Missing helper files used by syncing now recover automatically instead of failing permanently.
- Suggestion and feature request sharing was added in Settings as a separate section from app-specific feedback.
- The Settings suggestions form no longer shows the app log attachment option.
- The old Activity Log section was removed from Settings.
- Duplicate feedback submissions are blocked better, so repeated taps should not create extra entries.
- Install and uninstall status refreshes are more reliable after returning from Android system screens.
- Cached data handling was improved so the store can stay more stable when live content has a temporary issue.

## Permissions Required (For Users)

- `INTERNET`: required by the app on Android
- `POST_NOTIFICATIONS`: required by the app on Android
- `REQUEST_DELETE_PACKAGES`: required by the app on Android
- `REQUEST_INSTALL_PACKAGES`: required by the app on Android

## Privacy

This app is intended to use only the permissions needed for its core Android features.
It does not require file, photo, video, or audio storage access for normal use.
It does not declare contacts or location access in the Android manifest.

## Important Notes

- `Notifications` help the app show status updates and alerts.

## Supported Device

- Android only.
- Minimum Android version: Android 5.0 (API 21).

## How To Use

1. Install `Open_Store_ver_1.6.6.apk` on your Android device.
2. Open Open Store.
3. Grant any required permissions when prompted.
4. Use the app normally.

## How to Disable / Uninstall

1. No special disable steps are required for Open Store.
2. Uninstall Open Store normally from the launcher or Android Settings.

## Feedback

For general suggestions, new ideas, or improvements for Open Store itself, use the Feedback option in the Open Store Settings section.

For bug reports or new feature requests related to any app shown inside Open Store, use that app's own Feedback option from its app card or details view.
