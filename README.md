# LYNZ Android Releases

Private APK release assets and signed update metadata for 凌视 (LYNZ). Source code remains in KaiXiao55/src-lorat-vn-dockkit, branch android. APK files belong in Release assets, not Git history.

The website https://lynzrc.com provides the update API and authenticated tester download access. GitHub archival does not publish an app update: the controlled publisher verifies the artifact, then the owner reviews and publishes a channel through the existing MFA console.

| Artifact | Purpose | Application source commit |
| --- | --- | --- |
| 1.10.85 / code166 | Updater-capable bootstrap already cover-installed on the phone | 2fb751b2237bcaf5d4e646575b5ba761681e7632 |
| 1.10.86 / code167 | Same functional code, higher-version OTA acceptance target; not USB-installed | 3464672c399f8f7cb9fc17b74f5fa12efe769b3e |

Both use com.lynz.rcvision and the existing internal securityTest signer. Updates preserve data and require a safe idle state and user system confirmation. GitHub credentials, APK/update signing private keys and account credentials must never be stored in the app or this repository.

The release repository tag commit and application source commit are separate identifiers. Server publication remains a separate, audited owner action. Current artifacts are private internal tests, not a public/store distribution.
