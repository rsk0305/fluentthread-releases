# FluentThread release policy

Every update must publish both a versioned APK asset and this `release.json` manifest.

1. Increase Android `versionCode` and `versionName`.
2. Build with `https://raw.githubusercontent.com/rsk0305/fluentthread-releases/main/release.json` as the update manifest URL.
3. Create the matching GitHub release and upload the APK asset.
4. Update `release.json` with the new version, direct HTTPS APK URL, SHA-256, size, and notes.
5. Verify the manifest and APK URLs before announcing the release.

The Android client rejects incomplete, oversized, hash-mismatched, package-mismatched, signer-mismatched, or non-upgrade APKs.