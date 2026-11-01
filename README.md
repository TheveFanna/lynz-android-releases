# LYNZ Android Releases

Private release artifacts for 凌视 (LYNZ). APK files are stored only as GitHub Release assets, together with version notes and verification metadata.

Application source: KaiXiao55/src-lorat-vn-dockkit, branch android.
Update entry point: https://lynzrc.com (authenticated internal tester distribution).

GitHub archival does not publish a version to the app. The controlled publisher verifies an immutable APK and signed metadata, then the website owner selects a channel using the existing MFA console. GitHub credentials are never embedded in the app.

Bootstrap 1.10.85 / code166 uses package com.lynz.rcvision and the existing internal securityTest signer. Cover-install with adb install -r preserves app data. Later updates use the app's verified system-confirmed installer while idle. No APK signing keys, update-signing private keys or account credentials belong in this repository.

The release repository tag commit and application source commit are separate values. Bootstrap application source commit: 2fb751b2237bcaf5d4e646575b5ba761681e7632.
