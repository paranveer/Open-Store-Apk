# Open Store

<p align="center">
  <img src="assets/icons/open_store_icon.png" alt="Open Store Icon" width="140" />
</p>

Open Store is a Flutter Android app (`com.simba.openstore`) that fetches APKs from your GitHub repository, shows install/update status, verifies integrity, and supports feedback + telemetry sync.

## Features

- APK catalog from GitHub (direct mode) or backend API (proxy mode)
- Install status: installed/not installed + installed version
- Upgrade detection when repo version is newer
- Download with pause/resume/retry/redownload/delete APK
- Integrity checks (MD5/SHA1/SHA256/SHA512 + Git blob SHA1 fallback)
- Optional APK signer SHA-256 allowlist validation
- App-level feedback flow with status updates (`Not looked`, `Looking`, `Done`, `NA`)
- Download counters (`U` unique, `R` redownload) with `NOD.txt` sync
- Installed snapshot + telemetry sync support
- Theme modes: system, light, dark

## Expected Repo Data Layout

```text
Open_Store/
  Face Mirror/
    ver_1.0.0.apk
    ver_1.0.0.apk.sha1   (or .md5 / .sha256 / .sha512)
    README.md
    assets/
      icon.png
  Fingy/
    ver_1.0.0.apk
    ...
  NOD.txt
  Feedback.txt
  Installed.txt
```

### `NOD.txt` format

```text
Face Mirror : unique downloads : 0 | redownloads : 0
Fingy : unique downloads : 0 | redownloads : 0
Nature Heal : unique downloads : 0 | redownloads : 0
Neon Dodge : unique downloads : 0 | redownloads : 0
```

## Quick Start (Copy/Paste)

### 1) Flutter setup

```bash
flutter --version
flutter pub get
flutter analyze
flutter test
```

### 2) Build in Direct GitHub Mode (private repo access from app)

Use a GitHub PAT with repo read/write scopes.

```bash
TOKEN='your_github_pat_here'
B64=$(printf '%s' "$TOKEN" | base64 | tr -d '\n')

flutter build apk --debug \
  --dart-define=OPEN_STORE_GH_TOKEN_B64=$B64
```

Install:

```bash
adb install -r build/app/outputs/flutter-apk/app-debug.apk
```

### 3) Build in Backend Mode (recommended for production)

Run backend from [`backend/README.md`](backend/README.md), then build app with backend URL:

```bash
flutter build apk --release \
  --dart-define=OPEN_STORE_API_BASE_URL=https://your-api-domain.com
```

Optional backend write auth:

```bash
--dart-define=OPEN_STORE_BACKEND_WRITE_KEY=your_write_key
--dart-define=OPEN_STORE_BACKEND_SIGNING_SECRET=your_signing_secret
```

## Core Tech Notes

- App source root: `lib/`
- Main controller: `lib/src/controller/open_store_controller.dart`
- Direct GitHub service: `lib/src/services/github_store_service.dart`
- Backend proxy service: `lib/src/services/backend_store_service.dart`
- Local settings/token storage: `lib/src/services/settings_service.dart`

## Troubleshooting

- `GitHub API failed 403`:
  - Token missing/expired/insufficient scopes, or network policy blocking GitHub API.
- `HTTP 404` in backend mode:
  - Check backend env (`GITHUB_OWNER`, `GITHUB_REPO`, `GITHUB_BRANCH`, `GITHUB_TOKEN`).
- Download size appears larger than APK:
  - Resume/full-body handling has been fixed in current code. Rebuild + reinstall latest APK.
- `Sync pending: missing GitHub write token`:
  - Build with `OPEN_STORE_GH_TOKEN_B64` or configure backend write auth.

## Security Guidance

- For public user distribution, prefer backend mode so PAT stays server-side.
- Do not commit raw tokens to source control.
- Rotate tokens regularly.

## Package

- App name: `Open Store`
- Android package: `com.simba.openstore`
Jot something down
