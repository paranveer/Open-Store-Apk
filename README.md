<div align="center">
  <h1>Open Store</h1>
  <p><strong>Latest Available Version:</strong> 1.8.3</p>
  <p><strong>Build Date and Time(UST)</strong> 24-MAR-2026 02:59 AM</p>
  <p><strong>SHA1</strong> 9e757c2b050ed67ac1a5fa7f476b256e97f3fc9d</p>
  <p><strong>Platform</strong> Android</p>
</div>

![Open Store App Icon](assets/icons/open_store_icon.png)

## About the App

Open Store is an Android app that gives users one place to access apps developed for real-life challenges and everyday use. It brings multiple apps under the same hood, so users can discover, download, install, open, and update them from one store.

It is useful in real life when users want a single platform to explore and use apps such as:

- Reflectly
- Luma
- LumaFlash
- Control App Time
- Firm App Launch
- Fingy
- Nature Heal
- Neon Dodge
- 5 Sec
- More apps to come.

Common features include:
- browse all supported apps in one list
- download and install apps from one place
- open installed apps directly from the store
- see when a newer app version is available
- update apps from one place
- read important app details before downloading
- share app feedback for specific apps
- send suggestions and feature requests for Open Store itself
- verify version, build, and SHA1 details when needed

## Recent Fixes

- Internal source-system wording is now hidden better from normal users, so GitHub, README, manifest, and path-related terms should no longer appear in the app’s normal version details or error messages.
- The Open Store Settings screen no longer repeats `Current installed` version text in multiple places.
- Build date and time in the Open Store version summary now read correctly from the latest README format, including combined lines like `Build Date and Time(UST) ...`.
- Large app downloads now recover even when the uploaded `.apk.asset.json` file is missing the final GitHub Release asset URL. Open Store can resolve the correct release asset path more reliably, and future admin uploads preserve those URLs instead of overwriting them.
- Generated Open Store package files now use the current `Open_Store` release channel in their manifest and README download links, so future packaged releases should stop pointing to the older repo path.
- Open Store self-update downloads now recover more reliably when the update manifest has incomplete release URLs. The app now fills in the missing release asset path and prefers the authenticated release asset source in direct GitHub mode.
- App downloads now use a more reliable authenticated GitHub download path in direct mode, so store downloads should stop failing across apps in the private repo setup.
- Auto refresh now follows the interval selected in Settings. If you choose 5 minutes, the app should no longer refresh every few seconds.
- App icons are preserved better during refreshes, so they should not keep going on and off while the catalog updates.
- Open Store update downloads now show smoother progress while downloading.
- When an update download is paused, the app now shows the downloaded amount more accurately.
- Open Store update checks now refresh the latest catalog first, so newly pushed store updates should show up more reliably.
- Open Store update detection is now more tolerant of update package naming and file-format differences in the dedicated update folder.
- Build date and time are now shown together more clearly in the version details.
- The Open Store update card and version details now stay aligned more reliably, so installed version, latest version, and status are shown more consistently.
- Manual Open Store update checks now refresh the installed app version more reliably, so the update status should stay correct after you tap `Check for Open Store Update`.

## Recent Features

- Feedback sharing now supports an optional gallery image attachment.
- Suggestion and feature request sharing was added in Settings as a separate section from app-specific feedback.
- Each app section was redesigned to feel more raised and visually deeper, while staying usable on mobile screens.
- App actions were simplified with a cleaner overflow menu for secondary options.
- The details view now presents information in simpler grouped sections such as version, use case, features, permissions, and integrity.

## Download URL

- Direct latest APK download: [https://github.com/paranveer/Open_Store/releases/download/open-store-admin-large-files/Open_Store__Open_Store_ver_1.8.3.apk](https://github.com/paranveer/Open_Store/releases/download/open-store-admin-large-files/Open_Store__Open_Store_ver_1.8.3.apk)
- Release page: [https://github.com/paranveer/Open_Store/releases/tag/open-store-admin-large-files](https://github.com/paranveer/Open_Store/releases/tag/open-store-admin-large-files)
- Always download the latest available Open Store version.
- If the direct file link does not work for you, open the release page and download the newest APK shown there.

## Before You Start, Permissions & Privacy

- If you are installing the APK manually, allow `Install unknown apps` for the browser or file manager that opens it.
- Open the app after installation and grant the required Android permissions when prompted.

### Permissions Required

The app only requests the following Android permissions necessary for its functionality:

- `INTERNET` - enables network access required for the app to function
- `POST_NOTIFICATIONS` - allows the app to send status updates and alerts
- `REQUEST_DELETE_PACKAGES` - enables package management features when needed
- `REQUEST_INSTALL_PACKAGES` - allows installation-related actions when required

### Privacy and Important Notes

The app is designed to use only the permissions necessary for its core features and does not access unnecessary personal data.

It does **not** request or declare access to:
- Camera
- Microphone
- Contacts
- Location
- Storage (files, photos, videos, or audio)

The app does not access personal data beyond what is required for basic functionality.

**Important:**
Only grant permissions you are comfortable with. You can review or revoke permissions anytime from your Android device settings.

## Supported Device

- Android only.
- Minimum Android version: Android 5.0 (API 21).

## How To Use

1. Install `Open_Store_ver_1.8.3.apk` on your Android device.
2. Open Open Store.
3. Allow any required permissions when prompted.
4. Browse the available apps or open an app card to view details.
5. Use the available actions to download, install, update, or open supported apps.
6. Open Settings if you want to send suggestions or manage store options.

## How to Disable / Uninstall

1. No special disable steps are required for Open Store.
2. Uninstall Open Store normally from the launcher or Android Settings.

## Feedback

For general suggestions, new ideas, or improvements for Open Store itself, use the Feedback option in the Open Store Settings section.

For bug reports or new feature requests related to any app shown inside Open Store, use that app's own Feedback option from its app card or details view.
