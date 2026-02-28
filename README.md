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

## Security Guidance

- For public user distribution, prefer backend mode so PAT stays server-side.
- Do not commit raw tokens to source control.
- Rotate tokens regularly.

## Package

- App name: `Open Store`
- Android package: `com.simba.openstore`
Jot something down
